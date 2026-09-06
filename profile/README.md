# Welcome 👋

<div align="center">

**The production stage of a three-stage lifecycle.**

[![ANSELMES](https://img.shields.io/badge/ANSELMES-Production%20Estate-1f6feb?style=for-the-badge&logo=github&logoColor=white)][org]
[![License](https://img.shields.io/badge/License-GPL--3.0-4c1?style=for-the-badge)][gpl]

[![cicd](https://img.shields.io/github/v/release/anselmes/cicd?label=cicd&color=1f6feb)][cicd]
[![clact](https://img.shields.io/github/v/release/anselmes/clact?label=clact&color=1f6feb)][clact]
[![config](https://img.shields.io/github/v/release/anselmes/config?label=config&color=1f6feb)][config]
[![toolchain](https://img.shields.io/github/v/release/anselmes/toolchain?label=toolchain&color=1f6feb)][toolchain]

</div>

This page is the public face of the organization: what it is for, what is published
here, and what you can reasonably expect from it. Everything below concerns the
public repositories — internal working practice lives elsewhere.

## Table of Contents

- [1. 🧭 What this organization is](#1--what-this-organization-is)
- [2. 📦 What is public here](#2--what-is-public-here)
- [3. 🔁 Upstream mirrors](#3--upstream-mirrors)
- [4. 📄 Using this code](#4--using-this-code)
- [5. 🤝 Issues and contributions](#5--issues-and-contributions)
- [6. 📬 Contact](#6--contact)
- [License](#license)

## 1. 🧭 What this organization is

ANSELMES is the production estate. What it publishes is largely the machinery the
rest of the estate is built with — reusable CI/CD workflows, composite actions,
charts, images, and development tooling.

This organization occupies the final stage of a three-stage lifecycle:

1. **Exploration.** An idea begins as personal scratch work, outside this
   organization.
2. **Incubation.** Once it warrants sustained effort, it is built out, tested, and
   hardened — still outside this organization.
3. **Production.** When it matures, it is promoted here and development continues,
   with production use as the target. This is the work the organization exists for.

Two consequences are worth internalising. A repository arriving here has already
been through incubation, so it is not a first draft — and it has not stopped
moving either. **Production is what this work is being developed toward, not a
claim that every repository has already arrived.**

Most of the estate is private or internal, so what is visible from outside is a
deliberate slice rather than the whole of it. A reference to a repository you
cannot open is a repository you lack access to, not a dead link.

## 2. 📦 What is public here

Each repository carries its own README, and each is the place to start for the
ground it covers.

| Repository               | What it is                                                                          |
| ------------------------ | ----------------------------------------------------------------------------------- |
| [cicd][cicd]             | Reusable GitHub Actions workflows, development containers, and automation scripts   |
| [clact][clact]           | Composite actions for building, packaging, signing, and publishing artifacts        |
| [charts][charts]         | Helm charts, published as OCI artifacts                                             |
| [config][config]         | Configuration files and templates for development environments and system setup     |
| [toolchain][toolchain]   | Development environment, cluster bootstrap, security, and embedded hardware tooling |
| [images][images]         | Container image definitions built and published from this organization              |
| [zephyr-lang-swift][zls] | Swift language support for Zephyr RTOS, with CMake and Kconfig integration          |
| [repository][repository] | The repository scaffold used when starting new work                                 |

`repository` is the one scaffold still in use. The per-stack template repositories
this organization once published have been retired, and their documentation is no
longer maintained alongside them.

## 3. 🔁 Upstream mirrors

> [!NOTE]
> Most of the public repository list is mirrors, not original work. Roughly two
> dozen forks track upstream projects the estate builds from — kernel and
> bootloader sources, Yocto and OpenEmbedded layers, silicon and RISC-V projects,
> and networking appliances. They carry their upstream's licensing, conventions,
> and branch names rather than ours, issues and pull requests against them belong 
> upstream, and none of them is a pattern to follow for new work.

The full inventory, mirrors and archives included, is at <https://github.com/orgs/anselmes/repositories>.

## 4. 📄 Using this code

Everything published here is offered as-is, without warranty. Licensing differs
between the original repositories and the mirrors, so check before reusing
anything:

| Repository                             | Licence                                                              |
| -------------------------------------- | -------------------------------------------------------------------- |
| The original repositories in section 2 | GPL-3.0, with a `LICENSE` file in each                               |
| Upstream mirrors                       | Whatever the upstream sets — Apache-2.0, GPL-2.0, MIT, or undeclared |

Confirm a repository's default branch rather than assuming `main`. The original
repositories use it, but the mirrors variously build from `master`, `trunk`
(`meta-swift`) and `current` (`vyos-build`).

## 5. 🤝 Issues and contributions

Contributions are welcome on the original repositories, under the conventions the
estate applies everywhere: signed commits, sign-off enforced organization-wide,
`.editorconfig` honoured, and one subject per pull request. [CONTRIBUTING.md][contributing]
has the detail, and an individual repository may set its own policy that supersedes
it.

What is not promised is a response time. These repositories are maintained
alongside other work, review is best-effort, and no support commitment attaches to
an issue or a pull request.

Mirrors are the exception throughout: changes to them belong upstream, with the
project that owns the code.

> [!CAUTION]
> Never report a security vulnerability in a public issue or pull request. Use the
> private route described in [SECURITY.md][security].

## 6. 📬 Contact

| Route                              | Use it for                                        |
| ---------------------------------- | ------------------------------------------------- |
| <https://anselmes.com>             | The organization itself                           |
| <schubert@anselmes.com>            | General enquiries                                 |
| <git@anselm.es>                    | Security reports, access, and estate-wide matters |
| Issues on the repository concerned | Anything specific to one repository               |

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

[charts]: https://github.com/anselmes/charts
[cicd]: https://github.com/anselmes/cicd
[clact]: https://github.com/anselmes/clact
[config]: https://github.com/anselmes/config
[contributing]: https://github.com/anselmes/.github/blob/main/CONTRIBUTING.md
[gpl]: https://www.gnu.org/licenses/gpl-3.0
[images]: https://github.com/anselmes/images
[org]: https://github.com/anselmes
[repository]: https://github.com/anselmes/repository
[security]: https://github.com/anselmes/.github/blob/main/SECURITY.md
[toolchain]: https://github.com/anselmes/toolchain
[zls]: https://github.com/anselmes/zephyr-lang-swift
