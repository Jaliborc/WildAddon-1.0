# WildAddon-1.0 :computer:
A library heavily inspired in [AceAddon-3.0](https://www.wowace.com/projects/ace3), with small behavior changes and additional features that I needed and were incompatible with Ace. Requires [AceEvent-3.0](https://www.wowace.com/projects/ace3).

### Library API
|Name|Description|
|:--|:--|
| :Embed(object) | Adds the library method to your object. |
| :NewAddon(name [, object] [, libraries]) | Creates a public **addon object** or turns the provided one into it. |

### Addon API
Objects are initialized with [AceEvent-3.0](https://www.wowace.com/projects/ace3) methods already embedded. In addition to the ones provided by that library, addons and modules also have:

|Name|Description|
|:--|:--|
| :NewModule(name [, object] [, libraries]) | Same as `:NewAddon`, but creates a local **addon object**, called a module. |
| :RegisterSignal(id, call, [, args]) | Listens to an internal message among the addon and its modules. |
| :UnregisterSignal(id) | Stops listening to an internal module message. |
| :FireSignal(id, [, args]) | Sends an internal message to the addon and its modules. |
