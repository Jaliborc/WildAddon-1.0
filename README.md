# WildAddon-1.0 :computer:
[![Patreon](http://img.shields.io/badge/news%20&%20rewards-patreon-ff4d42)](https://www.patreon.com/jaliborc)
[![Paypal](http://img.shields.io/badge/donate-paypal-1d3fe5)](https://www.paypal.me/jaliborc)
[![Discord](http://img.shields.io/badge/discuss-discord-5865F2)](https://bit.ly/discord-jaliborc)

A library inspired by [AceAddon-3.0](https://www.wowace.com/projects/ace3), with small behavior changes and additional features that I needed and were incompatible with Ace. Requires [AceEvent-3.0](https://www.wowace.com/projects/ace3).

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

### :warning: Reminder!
If you use this library, please list it as one of your dependencies in the CurseForge admin system. It's a big help! :+1: