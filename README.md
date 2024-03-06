#  [Aegis JS Project](https://github.com/AegisJSProject/)

AegisJSProject is a GitHub Organization publishing Open Source libraries to offer minimal, web-stardards based modules that are framework an build tool agnistic.

## FAQ

**Is this yet another JavaScript Framework?**

No. Not really. This is a collection of rather minimal libraries, each addressing specific concerns/needs of web development.
While the collection of libraries as a whole might (and somewhat aims to) solve many of the same problems tyically addressed
by a "framwork", it aims to do so in a way that is stadards-based, as unopinionated as possible, compatible with any framework
you might already be using, and ultimately up to the developer to pick-and-choose what they want. For example, you could just
use the HTML Parser and Sanitizer (`@aegisjsproject/core/parsers/html.js`) without all the rest, and that is perfectly fine.

**Why  should I use this instead of [*insert framework or library here*]?**

Who said "instead of"? You can have and use both (probably). While this might eliminate the need for existing framewoks in
some cases, it does not aim to replace them. In fact, workking along side frameworks is just another reason why it's so
important that this be minimal in size - it'd be pretty reediculous if you had to load all of React just to use a React
component or two in an Angular project, but... loading maybe a few kb for however many web components that work in any
or no framework is pretty acceptable.

**How secure is this?**

It's not an instant, one-size-fits-all solution to all of your security woes... Let's just be upfront about that now.
*NOTHING* is! Security is multi-faceted, and very much depends on your threat model.

While Aegis makes a best effort to provide secure defaults and behavior, it should be understood more as being compatible with
an otherwise secure architecture. It aims to be compatible with a strict [`Content-Security-Policy`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Security-Policy)
and [TrustedTypes](https://developer.mozilla.org/en-US/docs/Web/API/trustedTypes),but does not and cannot protect against SQL
Injection, a weak CSP, a `TrustedTypesPolicy` that is too permissive, etc.
