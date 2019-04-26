# Think through Model, View, Controller, Model-Controller, View-Controller, View-Model

"If we have ViewControllers responsible for the View, then we can have ModelControllers responsible for the Model" - his example was NS/UIDocument reading/writing to database and updating observers.

And variants like MVVM

Apple has many types of controllers: Mediating Controller, Coordinating Controller, Model Controller, View Controller, Container View Controller. mediating controller mediates the flow of data between view objects and model objects. Coordinating controller's role in an application is to oversee--or coordinate--the functioning of the entire application or of part of the application.

Massive View Controller because ViewController combines View and Controller responsibilities, and model is often really small/light. So everything ends up in ViewController.

Not everything wraps up into a M, V, nor C. E.g. service layers: networking, database access, tracking, etc.

MVC doesn't structure your whole application, only the user-facing portion.

https://youtu.be/A1vzcxR-Ss0?t=69 and for slides: http://khd2.de/talks/MVC-Is-Not-Your-Problem/MVC_Is_Not_Your_Problem.pdf

Also read up on Apple's official doc on all this: https://developer.apple.com/library/archive/documentation/General/Conceptual/CocoaEncyclopedia/Model-View-Controller/Model-View-Controller.html and go into the specific patterns used, as https://blog.cocoafrog.de/2018/04/12/How-to-name-IBActions.html does.

![](../assets/2018-12-26-15-52-33.png)

![](../assets/2018-12-26-15-52-45.png)

# MV*
model fairly dumb, view fairly dumb. Something in the middle.

# Thoughts on MV*
In general, I very much like rules and guidelines. They usually make decisions ahead of time, so you can spend your decision energy on other things.

Probably better to think of it is Representation/Presentation, data/state, and events (wiring to init, then communication, user actions, and system operations to make dynamic)?

"Some of us apply the MVC (Model-View-Controller) pattern a bit too strictly. It's fine to create classes that are not models, views, or controllers. Really."  - Bart Jacobs

However, I think MV*/MVC has been taken too strictly. When writing code, if you are agonizing about whether this code belongs in the M, the V, or the C, then I think it is only hurting you. Especially because MVC doesn't cover all code responsibilites. What about helper **functions** that just convert some data to another format, where does that belong? What about a router and DI? Where do they fit?

MV* doesn't answer all questions: what about routing/DI? What handles device type/screen? (visual variation in View, context variation in controller, maybe). Looks like I said it before:

> MVC doesn't structure your whole application, only the user-facing portion.

And see here on [this](https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93presenter) MVP wikipedia page:

> MVP is a **user interface** architectural pattern engineered to facilitate automated unit testing and improve the separation of concerns in presentation logic:

I think MV* is a good thing to keep in mind when thinking about separating responsibilities and single responsibility principle, but I don't agree with any real firm implementations. Especially because I think MVC applies more to view (as components), with everything else fitting outside of MVC.

Instead, think about the scope of code.

This is one reason I like thinking in components, because they may have any amount of M, V, and/or C. Either the code is local and only concerned about this direct component or its children, or it is shared outside the scope of this component and should be considered shared.

Outside of components and scope, testability is a consideration (and a driving reason to think in MV*).