# Security Policy

This is the ANSELMES organization-wide default. It applies to every repository in
the organization that does not carry its own `SECURITY.md`, whatever that
repository's visibility, and any repository providing its own supersedes it.

The reporting route below is the same either way. What differs is context: on
private and internal repositories the member handbook governs day-to-day practice,
and this file is the disclosure route rather than the whole policy.

## What this code is

The repositories here are production-track infrastructure. They publish the CI/CD
workflows, composite actions, charts, images, and tooling that other work in the
estate is built with, which means a flaw in them can propagate into everything
downstream — a compromised action or a permissive workflow is worth more to an
attacker than a bug in any one application.

That is the reason to report. It is not a warranty: the code is offered as-is,
without support, and publication is not a claim of fitness for your purpose.

## Supported versions

Fixes land on a repository's default branch and roll into its next release. The
most recent release is the supported one — earlier tags are not backported, and
neither are forks you hold.

Several repositories publish no releases at all. For those, the tip of the default
branch is the only state that receives fixes.

If you are pinned to an older tag, moving forward is the remedy. Say so in your
report if you cannot, and we will tell you whether the fix is portable.

## Reporting a vulnerability

Two routes. Prefer the first.

**GitHub Security Advisories.** On the affected repository, open the **Security**
tab and choose **Report a vulnerability**. If that button is there, use it — it
opens a private advisory visible only to you and the maintainers, keeps the
discussion attached to the code in question, and is what a fix, a credit, and a CVE
are issued from later. The form lives at
`https://github.com/anselmes/<repository>/security/advisories/new`.

**Email.** Write to <git@anselm.es> if the Security tab offers no such button, if
the problem spans several repositories, or if you would rather not use GitHub.

> [!CAUTION]
> Never open a public issue or pull request for a security vulnerability, and do
> not post working exploit code in a public discussion.

Include whatever you have:

- The affected repository, and the commit or release you found it on.
- What the problem is, and the shortest path to reproducing it.
- What an attacker gains — the impact matters more than the severity label.
- Any mitigation or workaround you already know of.

A partial report is worth more than no report. Send what you have.

If you find a credential committed to a repository, report it the same way. Secret
scanning and push protection are enabled across the organization, but neither is
perfect. Any secret that reached a remote is treated as compromised and rotated,
whether or not it was ever live.

## What to expect

Reports are handled on a best-effort basis. There is no service-level agreement, no
guaranteed response time, and no bounty programme — these repositories are
maintained alongside other work. You will get an acknowledgement, and then either a
fix or an explicit decision not to fix.

Reporters are credited in the published advisory unless you ask us not to. Where a
finding warrants one, we will request a CVE through the advisory; GitHub is a CNA
and can assign directly from it.

## Disclosure

We publish the advisory once a fix exists, and tell you before it goes public.
Until then, please hold off on disclosing.

That request comes with a limit, because asking for silence while promising no
timeline would otherwise be open-ended. If ninety days pass from your report
without a fix and without a substantive response from us, consider yourself free to
publish. You do not need our permission, and we will not treat it as a hostile act.

## Out of scope

| Case                  | Where it belongs                                                      |
| --------------------- | --------------------------------------------------------------------- |
| Archived repositories | Not maintained. They are retained for reference and will not be fixed |
| Upstream mirrors      | Report to the upstream project, which owns the code                   |
| Retired templates     | Superseded and unmaintained; report against the code that replaced it |

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
