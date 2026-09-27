# Security Policy

## The short version

Do not open a public issue for a security problem. Email **contactopenax@gmail.com** with enough detail to reproduce, and you will get an acknowledgement within 72 hours and a triage decision within 7 days.

We ask for 90 days before public disclosure so a fix can ship. We do not run a bounty programme and we will not pretend otherwise.

## What is in scope

A polyfill for this API is a security boundary, not a convenience shim. It mediates who may call a tool, what they may pass to it, and what crosses back out. Treat a bug here as a bug in a trust boundary.

- Origin isolation. Can a document register, discover or execute a tool it should not reach, including through a cross-origin frame or a nested browsing context?
- `exposedTo` and `fromOrigins`. Can a tool be invoked by an origin that was not granted it, or can a granted origin reach a tool that was not exposed to it?
- Permissions Policy. Is the `tools` directive enforced, and does a disabled permission actually reject rather than quietly succeed?
- Tool execution. Can `executeTool` run a tool without the caller's own session, escalate privilege, or bypass a check the page author wrote?
- Injection. Can content from a page, a tool description or a tool argument reach a model in a way the page author did not intend to expose?
- Credentials. Can a secret, cookie or token cross the boundary between the page and an agent?
- Any shipped CLI, extension or test adapter that executes page-supplied data.

## What is out of scope

- Vulnerabilities in the web platform itself. Report those to the browser vendors.
- Vulnerabilities in Chromium's own WebMCP implementation. Report those to Chromium, and tell us anyway so we can track it.
- Weaknesses in the WebMCP design. Take those to [webmachinelearning/webmcp](https://github.com/webmachinelearning/webmcp/issues). We will still want to know, because our polyfill inherits the design.
- Missing hardening with no demonstrated path to exploitation. Suggest it in [Discussions](https://github.com/open-ax/ax-kit/discussions).
- Vulnerabilities in our dependencies. Report those upstream, and tell us which dependency so we can pin or drop it.

## Supported versions

| Version | Supported |
|---|---|
| 0.x | Best effort. Security fixes only, no backports to older minors. |

A 0.x package is a statement that the interface may still change. Pin what you depend on and read the release notes before upgrading.

## A note on this contact address

This is a personal address, not a role address. It works, and it is the truth of who maintains this today. Once a domain is registered it will be replaced with a `security@` alias so that reports do not depend on one person's willingness to keep reading mail.
