# Contributing to OpenAX

OpenAX is an independent implementation of [WebMCP](https://webmachinelearning.github.io/webmcp/), the [W3C Web Machine Learning Community Group](https://www.w3.org/community/webmachinelearning/) proposal that lets a web page declare typed tools for AI agents. The SDK lives in [ax-kit](https://github.com/open-ax/ax-kit).

## The rule that matters most

Every public API name must trace to a specific draft of the WebMCP specification. Do not invent names. Do not rename something because the name reads better. If the specification looks wrong to you, that is a discussion in [Discussions](https://github.com/open-ax/ax-kit/discussions) and an issue upstream at [webmachinelearning/webmcp](https://github.com/webmachinelearning/webmcp/issues), not a rename in the source.

If your change touches the tool surface, say which draft you implemented against. The draft is re-dated often and it changes underneath us, so an unpinned implementation cannot be reviewed.

## Before you start

Comment on the issue before you write code, so two people are not building the same thing. For anything larger than a bug fix, open a discussion first and agree on the shape before you write it.

## Pull requests

- One concern per pull request.
- Say which packages are affected and what a reviewer should look at first.
- Include the test that fails before your change and passes after it.
- Update the docs in the same pull request as the behaviour they describe.
- Say plainly if you could not verify something.

By contributing you agree that your work is licensed under [Apache-2.0](https://www.apache.org/licenses/LICENSE-2.0).

## AI-assisted contributions

Disclose it in the pull request description. Say which parts were generated and which you verified. A human is accountable for every line either way. Disclosure is not a reason to hold a change back, and undisclosed generated code is a reason to close one.

## Reporting something

Bugs and proposals go to [ax-kit issues](https://github.com/open-ax/ax-kit/issues). Questions go to [Discussions](https://github.com/open-ax/ax-kit/discussions). Security issues go to [SECURITY.md](https://github.com/open-ax/.github/blob/main/SECURITY.md) and nowhere else, because a public issue notifies everyone.

## Conduct

[CODE_OF_CONDUCT.md](https://github.com/open-ax/.github/blob/main/CODE_OF_CONDUCT.md). It applies in issues, pull requests, discussions and any specification work, and technical disagreement is covered by it as much as personal behaviour is.
