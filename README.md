# Cord Message

![CI Code Testing and Linting](https://github.com/cord-proj/cord-message/workflows/CI%20Code%20Testing%20and%20Linting/badge.svg)
![CI Security Audit on Push](https://github.com/cord-proj/cord-message/workflows/CI%20Security%20Audit%20on%20Push/badge.svg)

> Cord Message is an internal crate for the Cord Project. For more information and usage,
> check out [cord-proj/cord](https://github.com/cord-proj/cord).

The Message crate defines the message envelope and codec for transmitting messages over
the wire. It also provides a regex-like pattern matching module for comparing message
namespaces.

## FAQ

#### What is Cord?

Cord is a data streaming platform for composing, aggregating and distributing arbitrary
streams. To learn more about the project, check out
[cord-proj/cord](https://github.com/cord-proj/cord).

#### Why not use an off-the-shelf regex library?

Regex libraries will always provide more functionality for matching strings than this
library can. However what they cannot do is compare two regex patterns and determine
whether one encapsulates another, which is crucial to how publishers and subscribers
interact.
