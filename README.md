# Thinking about protocols with TLA+ and Apalache

In this workshop, we are introducing TLA+ and its model checkers:
TLC and Apalache. No prior knowledge of TLA+ is required.

## 1. Step-by-step instructions

### 1.1. Setup

If you want to reproduce the steps, make sure that you have installed
the following tools first:

 - [TLA Toolbox][] or [VScode plugin for TLA+][]
 - Apalache from the branch [igor/with-snowcat9][]. Check the Apalache
   manual on [Building Apalache from source][].
   If you are reading these lines after March 31, 2021, most likely,
   this branch has been merged into unstable and released as version
   0.15.0.
   Check [Apalache releases][].

### 1.2. Incremental specification of token transfer

Follow the [step-by-step instructions][].

**WARNING**: The final specification
[TokenTransfer8.tla](./examples/TokenTransfer8.tla) is **not** a
complete specification of [ICS20][].  If you want to specify [ICS20][],
you have to introduce the following features:

 - receiving (and sending) on (and to) coin source,
 - acknowledgments,
 - timeouts

## 2. Learning more about TLA+
 
 - [TLA+ Home Page][]
 - [TLA+ Video Course][]
 - [Specifying Systems][]
 - [TLA+ language manual for engineers][]
 - [LearnTla.com][]
 - [Community Modules][]
 - [TLC model checker][]
 - [TLA+ examples][]
    

[TLA+ examples]: https://github.com/tlaplus/examples
[TLA+ language manual for engineers]: https://apalache.informal.systems/docs/lang/index.html
[Apalache model checker]: https://apalache.informal.systems
[TLC model checker]: http://lamport.azurewebsites.net/tla/tools.html
[Summary of TLA]: https://lamport.azurewebsites.net/tla/summary.pdf
[TLA+ Home Page]: http://lamport.azurewebsites.net/tla/tla.html
[Specifying Systems]: http://lamport.azurewebsites.net/tla/book.html?back-link=learning.html
[Community Modules]: https://github.com/tlaplus/CommunityModules
[LearnTla.com]: https://learntla.com
[TLA+ Video Course]: http://lamport.azurewebsites.net/video/videos.html
[TLA Toolbox]: https://lamport.azurewebsites.net/tla/toolbox.html
[VScode plugin for TLA+]: https://marketplace.visualstudio.com/items?itemName=alygin.vscode-tlaplus
[igor/with-snowcat9]: https://github.com/informalsystems/apalache/tree/igor/with-snowcat9
[Building Apalache from source]: https://apalache.informal.systems/docs/apalache/installation/source.html
[Apalache releases]: https://github.com/informalsystems/apalache/releases
[step-by-step instructions]: ./docs/type-and-check.md 
[ICS20]: https://github.com/cosmos/ics/tree/master/spec/ics-020-fungible-token-transfer
