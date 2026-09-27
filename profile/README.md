<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./ax-mark-dark.png" />
    <img src="./ax-mark-light.png" alt="OpenAX" height="64" />
  </picture>
</p>

<p align="center"><b>the web was built for human eyes, we're fixing that for agents.</b></p>

<p align="center">
  <a href="https://webmachinelearning.github.io/webmcp/">WebMCP</a> ·
  <a href="https://github.com/open-ax/ax-kit">ax-kit</a> ·
  <a href="https://github.com/open-ax/ax-kit/discussions">Discussions</a> ·
  <a href="https://github.com/open-ax/.github/blob/main/CONTRIBUTING.md">Contributing</a> ·
  <a href="https://github.com/open-ax/.github/blob/main/SECURITY.md">Security</a> ·
  <a href="https://x.com/getaxkit">@getaxkit</a>
</p>

---

Agents use the web by looking at it. They screenshot the page, send the image to a model, and get back a coordinate to click. Then they do the whole thing again for the next step. Every observation re-buys the page as image tokens. Every action is a probabilistic guess. Any layout change, any breakpoint, any bot wall breaks the loop.

The page already knows. It knows which actions exist and what they take. It knows whether they can be undone and who is allowed to see the result. None of that survives a screenshot. That gap is the one worth closing: a page that tells an agent what it can do, in a form the agent can act on.

So the page says so itself. It registers typed tools. The browser mediates every call. The site's own code runs in the user's own session, in the user's own tab. The interface stays in sync because it is the same interface the user is already looking at. No pixels to interpret. No coordinates to guess. No second session to authenticate.

The result we want is an agent interaction as deterministic as the code underneath it. We want "did it work" answered by the page rather than inferred from pixels. We want a web where being legible to agents stops being a project you run and starts being a property of the page.

---

[WebMCP](https://webmachinelearning.github.io/webmcp/) is a Draft Community Group Report of the [W3C Web Machine Learning CG](https://www.w3.org/community/webmachinelearning/). OpenAX is an independent implementation. It is not affiliated with or endorsed by any of the W3C, Google, Microsoft or Apple.

Apache-2.0.
