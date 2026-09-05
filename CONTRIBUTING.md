# Contributing

This is the ANSELMES organization-wide default. It applies to every repository in
the organization that does not carry its own `CONTRIBUTING.md`, whatever that
repository's visibility.

If you are a member working in a private or internal repository, the member
handbook governs. What follows is addressed to contributors from outside the
organization.

## The default is open

The repositories here publish the machinery other work is built with — CI/CD
workflows, composite actions, charts, images, and development tooling. They are
meant to be used, and a problem you hit is worth reporting whether or not you
intend to fix it yourself.

So contributions are welcome by default. What is not offered alongside that:

- No service-level agreement. Review is best-effort, and a pull request may wait.
- No guaranteed response time on an issue.
- No support commitment. The code is offered as-is, without warranty.

This reflects available capacity rather than disinterest. The work is maintained
alongside other work, and an unanswered thread is a queue rather than a refusal.

## A repository may say otherwise

The default above is a floor, not a ceiling. Any repository is free to set its own
posture, and where it does, that posture governs. Precedence, highest first:

1. A `CONTRIBUTING.md` in the repository itself, which supersedes this file
   entirely.
2. A contribution policy stated in the repository's README.
3. This file.

Check the repository before assuming the default applies.

## What applies to a contribution

Sign-off is enforced organization-wide, so a commit without it is rejected at push
rather than flagged in review. The rest are conventions you are expected to follow.

| Requirement    | What it means                                                                       |
| -------------- | ----------------------------------------------------------------------------------- |
| Default branch | Confirm it rather than assuming `main` — the upstream mirrors vary                  |
| Editor config  | Honour the repository's `.editorconfig`; do not reformat around it                  |
| Signed commits | Commits are expected to be signed — see [signature verification][signing]           |
| Sign-off       | Enforced organization-wide, web edits included — see the [sign-off policy][signoff] |
| Licensing      | Original repositories are GPL-3.0, and contributions are accepted under those terms |

Keep a pull request to one subject, and describe what you changed and why. A change
that alters behaviour should say how you verified it — for a workflow or an action,
that means a link to a run where it did the right thing.

Upstream mirrors are the exception throughout: they follow their upstream's
licensing and conventions, and changes belong upstream rather than here.

## Security issues

> [!CAUTION]
> Never report a security vulnerability through a pull request or a public issue.
> Use the private route in [SECURITY.md][security].

## License

Copyright (c) 2026 Schubert Anselme <schubert@anselm.es>

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <https://www.gnu.org/licenses/>.

[security]: https://github.com/anselmes/.github/blob/main/SECURITY.md
[signing]: https://docs.github.com/en/authentication/managing-commit-signature-verification
[signoff]: https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/managing-the-commit-signoff-policy-for-your-repository
