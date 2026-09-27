<!--
Thanks for contributing. Two things are genuinely required rather than optional:
the specification draft you targeted, and how you verified the change.
Both are short to write and impossible to reconstruct later.
-->

### What this changes

<!-- One or two sentences. The problem it solves, not a restatement of the diff. -->

### Specification alignment

<!--
Required if this touches tool registration, discovery, execution, schemas,
annotations, or the origin and permission model.

Name the exact draft you implemented against. The draft is re-dated often, so
"latest" is not an answer.

If it does not touch the surface above, write "not applicable".
-->

Draft or commit implemented against:

### Packages affected

<!-- @ax-kit/* packages, or "none". -->

### How this was verified

<!--
The test that fails without your change and passes with it. If you could not
verify something, say which part and why. An unverified claim labelled as
unverified is fine. A gap presented as a result is not.
-->

### Checklist

- [ ] The test above exists and fails without this change
- [ ] Every new or renamed public API name traces to a dated specification draft
- [ ] Documentation changed in the same commit as the behaviour it describes
- [ ] `CHANGELOG.md` updated if this is user-visible
- [ ] I have disclosed below whether AI tooling was used

### AI tooling

<!--
Which parts were generated, which you reviewed, and what you verified by hand.
Disclosure is not a reason to hold a change back. Undisclosed generated code
is a reason to close the pull request.
-->

### Security

<!--
If this touches origin isolation, `exposedTo` or `fromOrigins`, the Permissions
Policy `tools` directive, or anything crossing the boundary between the page and
an agent, say so and describe the threat you considered. Otherwise "none".
-->
