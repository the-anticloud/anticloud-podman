# PODMAN

![license](https://img.shields.io/badge/license-license-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-infra_devops-lightgrey)

> Anticloud-hardened packaging of the upstream project `PODMAN` in category **INFRA DEVOPS**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** INFRA DEVOPS · **Upstream:** https://github.com/podman-container-tools/podman · **Upstream pin:** `3f04d208a3964d0e16d6d7b995c0ae30bf9fe38d` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

![PODMAN logo](https://raw.githubusercontent.com/containers/common/main/logos/podman-logo-full-vert.png)

# Podman: A tool for managing OCI containers and pods
![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)
![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/containers/podman)
[![Go Report Card](https://goreportcard.com/badge/github.com/containers/podman/v6)](https://goreportcard.com/report/github.com/containers/podman/v6)
[![OpenSSF Best Practices](https://www.bestpractices.dev/projects/10499/badge)](https://www.bestpractices.dev/projects/10499)

[![LFX Health Score](https://insights.linuxfoundation.org/api/badge/health-score?project=podman-container-tools&projects=https://github.com/containers/podman)](https://insights.linuxfoundation.org/project/podman-container-tools/project/containers-podman)
[![LFX Contributors](https://insights.linuxfoundation.org/api/badge/contributors?project=podman-container-tools&projects=https://github.com/containers/podman)](https://insights.linuxfoundation.org/project/podman-container-tools/project/containers-podman)

<br/>

Podman (the POD MANager) is a tool for managing containers and images, volumes mounted into those containers, and pods made from groups of containers.
Podman runs containers on Linux, but can also be used on Mac and Windows systems using a Podman-managed virtual machine.
Podman is based on libpod, a library for container lifecycle management that is also contained in this project. The libpod library provides APIs for managing containers, pods, container images, and volumes.

Podman releases a new major or minor release 4 times a year, during the second week of February, May, August, and November. Patch releases are more frequent and may occur at any time to get bugfixes out to users. All releases are PGP signed. Public keys of members of the team approved to make releases are located [here](https://github.com/containers/release-keys/tree/main/podman).

Only the most recent release receives upstream support. Exceptions are sometimes made in which case we offer a LTS version, the supported versions can be found [here](https://github.com/podman-container-tools/community/blob/main/SUPPORT.md#long-term-support-lts-versions)

* Continuous Integration:
  * [![Build Status](https://github.com/containers/podman/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/containers/podman/actions/workflows/ci.yml?query=branch%3Amain)
  * [GoDoc: ![GoDoc](https://godoc.org/github.com/containers/podman/libpod?status.svg)](https://godoc.org/github.com/containers/podman/libpod)
  * [Downloads](DOWNLOADS.md)

## Overview and scope

At a high level, the scope of Podman and libpod is the following:

* Support for multiple container image formats, including OCI and Docker images.
* Full management of those images, including pulling from various sources (including trust and verification), creating (built via Containerfile or Dockerfile or committed from a container), and pushing to registries and other storage backends.
* Full management of container lifecycle, including creation (both from an image and from an exploded root filesystem), running, checkpointing and restoring (via CRIU), and removal.
* Full management of container networking, using Netavark.
* Support for pods, groups of containers that share resources and are managed together.
* Support for running containers and pods without root or other elevated privileges.
* Resource isolation of containers and pods.
* Support for a Docker-compatible CLI interface, which can both run containers locally and on remote systems.
* No manager daemon, for improved security and lower resource utilization at idle.
* Support for a REST API providing both a Docker-compatible interface and an improved interface exposing advanced Podman functionality.
* Support for running on Windows and Mac via virtual machines run by `podman machine`.

## Roadmap

The future of Podman feature development can be found in its **[roadmap](ROADMAP.md)**.

## Communications

If you think you've identified a security issue in the project, please *DO NOT* report the issue publicly via the GitHub issue tracker, mailing list, or IRC.
Instead, send an email with as many details as possible to `security@lists.podman.io`. This is a private mailing list for the core maintainers.

For general questions and discussion, please use Podman's
[channels](https://podman.io/community/#slack-irc-matrix-and-discord).

For discussions around issues/bugs and features, you can use the GitHub
[issues](https://github.com/containers/podman/issues)
and
[PRs](https://github.com/containers/podman/pulls)
tracking system.

There is also a [mailing list](https://lists.podman.io/archives/) at `lists.podman.io`.
You can subscribe by sending a message to `podman-join@lists.podman.io` with the subject `subscribe`.

### Community Meetings

All Podman meetings are open to everyone, free to attend, and hosted via Zoom through the CNCF/Linux Foundation.
The full calendar is available on the [Podman Container Tools LFX Meetings page](https://zoom-lfx.platform.linuxfoundation.org/meetings/podman-container-tools?view=month).
Registering for a meeting sends you an invite for that meeting and all subsequent recurring instances.

| Meeting | Schedule | Format |
|---------|----------|--------|
| [Podman Community Meeting](https://zoom-lfx.platform.linuxfoundation.org/meeting/97486138230?password=3144ae43-0fd5-457e-a495-bb4e0202e9c2) and its [agenda](https://hackmd.io/fc1zraYdS0-klJ2KJcfC7w?both) | First **Tuesday of even-numbered months** (Feb, Apr, Jun, Aug, Oct, Dec) at **11:00 a.m. Eastern** (UTC-4 summer / UTC-5 winter) | ~1 hour — demos, announcements, and community updates |
| [Podman Monday Office Hours](https://zoom-lfx.platform.linuxfoundation.org/meeting/92776077694?password=deea5903-07a5-4e4d-9ad9-a6f52319fabe) and its [agenda](https://hackmd.io/@TomSweeneyRedHat/H1qIC9nkMe) | Every **Monday at 10:30 a.m. Eastern

*(excerpt; full text in `UPSTREAM_CLONE/`)*

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **C/C++ / Make** (manifests: Makefile; scanned in UPSTREAM_CLONE)
- Top-level source layout: `cmd/`, `completions/`, `contrib/`, `docker/`
- Snapshot size: **572 files**, **35712 lines of code** (measured; see Benchmarks)
- Primary languages: `.go` (281), `.md` (153), `.1` (49), `(none)` (21), `.in` (13), `.sh` (9)
- Upstream commit pinned for this packaging: `3f04d208a3964d0e16d6d7b995c0ae30bf9fe38d`

---

## Installation

* [GoDoc: ![GoDoc](https://godoc.org/github.com/containers/podman/libpod?status.svg)](https://godoc.org/github.com/containers/podman/libpod)
  * [Downloads](DOWNLOADS.md)

*Section quoted from the upstream readme.*
Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

[channels](https://podman.io/community/#slack-irc-matrix-and-discord).

For discussions around issues/bugs and features, you can use the GitHub
[issues](https://github.com/containers/podman/issues)
and
[PRs](https://github.com/containers/podman/pulls)
tracking system.

There is also a [mailing list](https://lists.podman.io/archives/) at `lists.podman.io`.
You can subscribe by sending a message to `podman-join@lists.podman.io` with the subject `subscribe`.

*Section quoted from the upstream readme.*
Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

[![LFX Contributors](https://insights.linuxfoundation.org/api/badge/contributors?project=podman-container-tools&projects=https://github.com/containers/podman)](https://insights.linuxfoundation.org/project/podman-container-tools/project/containers-podman)

<br/>

Podman (the POD MANager) is a tool for managing containers and images, volumes mounted into those containers, and pods made from groups of containers.
Podman runs containers on Linux, but can also be used on Mac and Windows systems using a Podman-managed virtual machine.
Podman is based on libpod, a library for container lifecycle management that is also contained in this project. The libpod library provides APIs for managing containers, pods, container images, and volumes.

Podman releases a new major or minor release 4 times a year, during the second week of February, May, August, and November. Patch releases are more frequent and may occur at any time to get bugfixes out to users. All releases are PGP signed. Public keys of members of the team approved to make releases are located [here](https://github.com/containers/release-keys/tree/main/podman).

Only the most recent release receives upstream support. Exceptions are sometimes made in which case we offer a LTS version, the supported versions can be found [here](https://github.com/podman-container-tools/community/blob/main/SUPPORT.md#long-term-support-lts-versions)

* Continuous Integration:
  * [![Build Status](https://github.com/containers/podman/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/containers/podman/actions/workflows/ci.yml?query=branch%3Amain)
  * [GoDoc: ![GoDoc](https://godoc.org/github.com/containers/podman/libpod?status.svg)](https://godoc.org/github.com/containers/podman/libpod)
  * [Downloads](DOWNLOADS.md)

*Section quoted from the upstream readme.*
---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | C/C++ / Make |
| Manifests detected | Makefile |
| Files in snapshot | 572 |
| Lines of code | 35712 |
| Dependency references | 0 |
| Upstream license | Apache-2.0 |
| Overlay license | Anticommons 0.1.0 |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

A little configuration by an administrator is required before rootless Podman can be used, the necessary setup is documented [here](https://github.com/containers/podman/blob/main/docs/tutorials/rootless_tutorial.md).

*Section quoted from the upstream readme.*
Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

*Excerpt from upstream `CONTRIBUTING.md`:*

![PODMAN logo](https://raw.githubusercontent.com/containers/container-libs/main/common/logos/podman-logo-full-vert.png)
# Podman Contributing Guide

We'd love to have you join the community!

Please first read our organization wide contributing guide: https://github.com/podman-container-tools/community/blob/main/CONTRIBUTING.md.
It contains all the general recommendations on how to work with issues and how to create proper commits and PRs for the Project.
Below you find helpful advice specific to only the Podman project.

## Topics

* [Contributing to Podman](#contributing-to-podman)
* [Libraries](#libraries)
* [Codebase structure](#codebase-structure)
* [Testing](#testing)
* [Documentation](#documentation)
* [Continuous Integration](#continuous-integration) [![Build Status](https://github.com/podman-container-tools/podman/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/podman-container-tools/podman/actions/workflows/ci.yml?query=branch%3Amain)

## Contributing to Podman

This section describes how to make a contribution to Podman.
These instructions are geared towards using a Linux development machine, which is required for doing development on the Podman backend.
Development for the Windows and Mac clients can also be done on those operating systems.
Check out these instructions for building the Podman client on [MacOSX](./build_osx.md) or [Windows](./build_windows.md).

> **Note:** Podman 6 dropped support for darwin/amd64 (Intel Mac) binaries. The macOS client is only available for darwin/arm64 (Apple Silicon). Attempting to build with `GOOS=darwin GOARCH=amd64` will fail on any host.

### Prepare your environment

Read the [install documentation to see how to install dependencies](https://podman.io/getting-started/installation#build-and-run-dependencies).

The install documentation will illustrate the following steps:
- Installation of required libraries and tools
- Installing Podman from source

The minimum version of Golang required to build Podman is contained in [go.mod](https://github.com/podman-container-tools/podman/blob/main/go.mod#L5).
You will need to make sure your system's Go compiler is at least this version using the `go version` command.

### Fork and source Podman

First, you need to fork this project on GitHub.
Then source your fork locally:
```shell
$ git source git@github.com:<you>/podman
$ cd ./podman/
```

### Using the Makefile

Podman uses a Makefile for common actions such as compiling Podman, building the d

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: Apache-2.0** (evidence: `LICENSE` in the upstream snapshot).

License file excerpt:

```text
                                 Apache License
                           Version 2.0, January 2004
                        https://www.apache.org/licenses/

   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION

   1. Definitions.

      "License" shall mean the terms and conditions for use, reproduction,
      and distribution as defined by Sections 1 through 9 of this document.

      "Licensor" shall mean the copyright owner or entity authorized by
      the copyright owner that is granting the License.

      "Legal Entity" shall mean the union of the acting entity and all
      other entities that control, are controlled by, or are under common
      control with that entity. For the purposes of this definition,
      "control" means (i) the power, direct or indirect, to cause the
      direction or management of such entity, whether by contract or
      otherwise, or (ii) ownership of fifty percent (50%) or more of the
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original Apache-2.0 terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `Apache-2.0` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `PODMAN` (category: INFRA DEVOPS)
- **Upstream URL:** https://github.com/podman-container-tools/podman
- **Pinned commit (SHA):** `3f04d208a3964d0e16d6d7b995c0ae30bf9fe38d`
- **Branch:** main
- **Pin provenance:** GitHub API commits/main. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`a5efed89c9deb3ba1c14e42486cb0903e8c1c97486384c2731b775b6f0323d15`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe and Mail, Business Insider, National Post, Financial Post, StreetInsider, Digital Journal, Barchart, International Business Times, and fox47 · National Law Review.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

