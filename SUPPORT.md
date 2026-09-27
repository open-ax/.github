# Support

## Where to ask

| If your question is about | Ask it in |
|---|---|
| How do I use this, or does it work the way I expect | [Discussions on ax-kit](https://github.com/open-ax/ax-kit/discussions) |
| Something is broken, or a tool does not do what the specification says | [Issues on ax-kit](https://github.com/open-ax/ax-kit/issues) |
| A specification change you want to argue for | [Issues on webmachinelearning/webmcp](https://github.com/webmachinelearning/webmcp/issues) |
| A security vulnerability | **Not** a public issue. See [SECURITY.md](https://github.com/open-ax/.github/blob/main/SECURITY.md) |

Prefer Discussions for anything that is not clearly a bug. A question in an issue tracker is harder to answer in public, which helps the next person who has it, and there is no guaranteed response time on either.

## Before you open anything

The most common cause of a confusing report is the browser rather than the library. WebMCP is an origin trial, so whether `document.modelContext` exists changes what your code is allowed to do. Saying which of these you are on saves a round trip:

- Chromium with the origin trial enabled, so the API is native
- Chromium without it, so a polyfill is doing the work
- Any other browser, so a polyfill is doing the work

If the specification and the implementation disagree, that is a real finding and the most valuable kind of report this project can receive. Please include the draft date or commit you were reading, because the draft changes.

## What to expect

This is a project maintained in spare time by one person. There is no support contract and no response-time commitment. Reports are read, and the ones that are actionable get fixed, in roughly the order they arrive.

That is not a reason not to report something. It is a reason to make the report cheap to act on: what you did, what you expected, what happened instead, and the smallest thing that reproduces it.

## Elsewhere

- [Contributing](https://github.com/open-ax/.github/blob/main/CONTRIBUTING.md) if you want to send code
- [Code of conduct](https://github.com/open-ax/.github/blob/main/CODE_OF_CONDUCT.md) for how we treat each other
- [@getaxkit](https://x.com/getaxkit) for release notes
