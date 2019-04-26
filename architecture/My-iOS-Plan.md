# Core + UI
## Core
Core is anything in the `Foundation` level (also includes Core Data, Cloud Kit, etc). Communication is done via `Operation`s. If I made a universal app, this is the part that would likely be shareable to iOS, AppleTV, Mac, WatchOS, etc.

Core encapsulates the Model Domain and interacting with the system/services. Rather importantly, it uses Core Data and its ManagedObjects.

## UI
UI is essentially a side effect of state.

Why seperate view's state from view? Testability is the only good reason I can think of.

UI is the interface that a user will interact with. Views use ManagedObjects (+ extensions to make up a ViewModel) and local state via properties. User actions may affect just the View, or be sent out to core via an operation (in the controller).

So, ManagedObjects become the ViewModel, or at least a part of it. I plan to unit test these extensions which essentially just format.

ViewController is responsible for rendering UI (init/setup and updates), which includes layout and animation. Also responsible for handling actions.

VCs observe managedObjectContext to update UI.

setup() vs update(): setup() only called once. Better yet, use render() to accomplish both (so smart of React to name it this).

# UIView vs UIViewController
Use UIView if it is a single, logical unit. For example, `Icon` makes sense even though it internally uses a couple views. Either way, they act like one.
- Out view constraints should always be set by parent.
- Should only be used for leaf nodes

UIView is-a view. UIViewController has-a view.

UIViewController is primary "component" view because it can embed other ViewControllers. This is the main reason to not go with UIView as the default "component".

# Cache
NSManagedObjectContext is the cache.

ViewControllers ONLY talk to cache. AKA all UI feeds from Core Data, not the network.
- separate network service to sync and observe cache w/ server

ViewControllers use NSFetchedResulsController for synced/always-updated cache dat

# Operations
Use operations for Core tasks.

Each operation does one, small, discrete unit of work.

Operation sin a queue
- unit test runs on main thread. Just call `operation.start()`.
- can report speeds (time diff state's start vs. end)
- can prioritize based on bandwidth

# Other rules
- Don't access AppDelegate directly
- Disconnect data collection and data display