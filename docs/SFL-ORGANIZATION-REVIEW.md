# Organization pull request review

This repository uses the reviewer tier from hemsoft-dev's signed SFL release `2.1.0-rc.21`. The installed source pin is `89425320ace3127a829d86e3b642fe2b31fd979e`.

Request a registered review for an open pull request with:

```sh
gh sfl review --repo hemsoft-dev/n8n-workflows --pr NUMBER
```

The strict `SFL Reviewer Gate Runner` check accepts authenticated Codex evidence for the current head, base and registered request. Pending requests, findings and changed context keep the gate closed. After a base advance, publish a new head and request a fresh review.

Use `gh sfl status --repo hemsoft-dev/n8n-workflows` to inspect the installed package and gate. Sync through a pull request with `gh sfl sync --repo hemsoft-dev/n8n-workflows --pr`; retain existing repository protections and additions.
