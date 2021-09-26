# LibEventDispatcher

```lua
-- This is a singleton.
local EventDispatcher = LibStub("EventDispatcher")

EventDispatcher.addEventListener(
    eventName , --[[ string: the name of the event ]]
    callbackFunc, --[[ function(table): the callback function, the argument is the data passed by the sender ]]
    prepend, --[[ bool: whether to prepend the event handler or append (default) it to the list of handlers ]]
)

EventDispatcher.dispatchEvent(
    eventName , --[[ string: the name of the event ]]
    data --[[ table|nil: data to make available to the event handlers, this is optional ]]
)

```