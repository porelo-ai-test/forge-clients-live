# forge-clients-live

Fixtures for [porelo-forge-clients](https://github.com/porelo-ai/porelo-forge-clients)' live checks against GitHub.
**Do not change by hand.**

The live check of the `github` client reads what this repository keeps for it - a pull request with an approving
review, comments and a resolved thread, a check run and a hook - in strict reading, and dispatches the workflow
`Fixture` to read its run, job and log. A change here, or a comment on the kept pull request, makes that check fail.
The recording test of porelo-forge-clients creates and removes what it needs itself.
