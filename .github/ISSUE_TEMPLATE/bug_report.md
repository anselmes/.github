---
name: Bug report
about: Something in a repository does not work as its README describes
title: ""
labels: bug
assignees: ""
---

<!--
Contributions and reports are welcome, but review is best-effort and no response
time is promised. See CONTRIBUTING.md.

Do NOT report a security vulnerability here. Use the Security tab on the affected
repository, or email git@anselm.es. See SECURITY.md.

For an upstream mirror (linux, u-boot, zephyr, edk2, the meta-* layers, and the
rest), report the problem to the upstream project instead — the code is theirs.
-->

## Where

- Repository:
- Release or commit (`git rev-parse --short HEAD`):
- Branch, if not the default:

## What happens

A short description of the behaviour, and what you expected instead.

## How to reproduce

The commands you ran, in order. A shell transcript is worth more than prose.

```shell

```

## Environment

Host OS and architecture, plus whichever of the following applies:

- **cicd**, **clact** — runner OS and label, plus a link to the workflow run
- **charts** — helm, kubectl, and Kubernetes server versions; Flux if in use
- **config**, **toolchain** — host OS and shell, plus the script or target invoked
- **images** — docker or podman version, and the target platform
- **zephyr-lang-swift** — Zephyr and west versions, Swift toolchain, target board

## Output

Build log, workflow log, `dmesg`, serial console, or `kubectl` output, as text in a
code fence rather than a screenshot — it needs to be searchable.

```text

```

## Anything you already tried

Workarounds, related issues upstream, or a diagnosis if you have one. Optional.
