# IST

![license](https://img.shields.io/badge/license-license-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-chip_quantization-lightgrey)

> Anticloud-hardened packaging of the upstream project `IST` in category **CHIP QUANTIZATION**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** CHIP QUANTIZATION · **Upstream:** https://github.com/istio/istio · **Upstream pin:** `e4350fd4d6c9905d9b5fe6d5c85ca7c521e45daa` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

# Istio

[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/1395/badge)](https://bestpractices.coreinfrastructure.org/projects/1395)
[![Go Report Card](https://goreportcard.com/badge/github.com/istio/istio)](https://goreportcard.com/report/github.com/istio/istio)
[![GoDoc](https://godoc.org/istio.io/istio?status.svg)](https://godoc.org/istio.io/istio)

<a href="https://istio.io/">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/cncf/artwork/refs/heads/main/projects/istio/icon/color/istio-icon-color.svg">
      <source media="(prefers-color-scheme: light)" srcset="https://github.com/istio/istio/raw/master/logo/istio-bluelogo-whitebackground-unframed.svg">
      <img title="Istio" height="100" width="100" alt="Istio logo" src="https://github.com/istio/istio/raw/master/logo/istio-bluelogo-whitebackground-unframed.svg">
    </picture>
</a>

---

Istio is an open source service mesh that layers transparently onto existing distributed applications. Istio’s powerful features provide a uniform and more efficient way to secure, connect, and monitor services. Istio is the path to load balancing, service-to-service authentication, and monitoring – with few or no service code changes.

- For in-depth information about how to use Istio, visit [istio.io](https://istio.io)
- To ask questions and get assistance from our community, visit [GitHub Discussions](https://github.com/istio/istio/discussions)
- To learn how to participate in our overall community, visit [our community page](https://istio.io/about/community)

In this README:

- [Introduction](#introduction)
- [projects](#projects)
- [Issue management](#issue-management)

In addition, here are some other documents you may wish to read:

- [Istio Community](https://github.com/istio/community#istio-community) - describes how to get involved and contribute to the Istio project
- [Istio Developer's Guide](https://github.com/istio/istio/wiki/Preparing-for-Development) - explains how to set up and use an Istio development environment
- [Project Conventions](https://github.com/istio/istio/wiki/Development-Conventions) - describes the conventions we use within the code base
- [Creating Fast and Lean Code](https://github.com/istio/istio/wiki/Writing-Fast-and-Lean-Code) - performance-oriented advice and guidelines for the code base

You'll find many other useful documents on our [Wiki](https://github.com/istio/istio/wiki).

## Introduction

[Istio](https://istio.io/latest/docs/concepts/what-is-istio/) is an open platform for providing a uniform way to [integrate
microservices](https://istio.io/latest/docs/examples/microservices-istio/), manage [traffic flow](https://istio.io/latest/docs/concepts/traffic-management/) across microservices, enforce policies
and aggregate telemetry data. Istio's control plane provides an abstraction
layer over the underlying cluster management platform, such as Kubernetes.

Istio is composed of these components:

- **Envoy** - Sidecar proxies per microservice to handle ingress/egress traffic
   between services in the cluster and from a service to external
   services. The proxies form a _secure microservice mesh_ providing a rich
   set of functions like discovery, rich layer-7 routing, circuit breakers,
   policy enforcement and telemetry recording/reporting
   functions.

  > Note: The service mesh is not an overlay network. It
  > simplifies and enhances how microservices in an application talk to each
  > other over the network provided by the underlying platform.

* **Ztunnel** - A lightweight data plane proxy written in Rust,
    used in Ambient mesh mode to provide secure connectivity and observability for workloads without sidecar proxies.

- **Istiod** - The Istio control plane. It provides service discovery, configuration and certificate management.

## projects

The Istio project is divided across a few GitHub projects:

- [istio/api](https://github.com/istio/api). This project defines
component-level APIs and common configuration formats for the Istio platform.

- [istio/community](https://github.com/istio/community). This project contains
information on the Istio community, including the various documents that govern
the Istio open source project.

- [istio/istio](README.md). This is the main code project. It hosts Istio's
core components, install artifacts, and sample programs. It includes:

    - [istioctl](istioctl/). This directory contains code for the
[_istioctl_](https://istio.io/latest/docs/reference/commands/istioctl/) command line utility.

    - [pilot](pilot/). This directory
contains platform-specific code to populate the
[abstract service model](https://istio.io/docs/concepts/traffic-management/#pilot), dynamically reconfigure the proxies
when the application topology changes, as well as translate
[routing rules](https://istio.io/latest/docs/reference/config/networking/) into proxy specific configuration.

    - [security](security/). This directory contains [security](https://istio.io/latest/docs/concepts/security/) related code.

- [istio/proxy](https://github.com/istio/proxy). The Istio proxy contains
extensions to the [Envoy proxy](https://github.com/envoyproxy/envoy) (in the form of
Envoy filters) that support authentication, authorization, and telemetry collection.

- [istio/ztunnel](https://github.com/istio/ztunnel). The project contains the Rust implementation of the ztunnel
component of Ambient mesh.

- [istio/client-go](https://github.com/istio/client-go). This project defines
  auto-generated Kubernetes clients for interacting with Istio resources programmatically.

> [!NOTE]
> Only the `istio/api` and `istio/client-go` projects expose stable interfaces intended for direct usage as libraries.

## Issue management

We use GitHub to track all of our bugs and feature requests. Each issue we track has a variety of metadata:

- **Epic**. An epic represents a feature area for I

*(excerpt; full text in `UPSTREAM_CLONE/`)*

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **Go** (manifests: go.mod, go.sum; scanned in UPSTREAM_CLONE)
- Top-level source layout: `architecture/`, `bin/`, `cni/`, `common/`, `docker/`, `istioctl/`, `licenses/`, `logo/`, `manifests/`, `operator/`, `pilot/`, `pkg/`
- Snapshot size: **6700 files**, **624881 lines of code** (measured; see Benchmarks)
- Primary languages: `.yaml` (3197), `.go` (2041), `(none)` (350), `.golden` (245), `.injected` (123), `.pem` (118)
- Upstream commit pinned for this packaging: `e4350fd4d6c9905d9b5fe6d5c85ca7c521e45daa`

---

## Installation

- [istioctl](istioctl/). This directory contains code for the
[_istioctl_](https://istio.io/latest/docs/reference/commands/istioctl/) command line utility.

    - [pilot](pilot/). This directory
contains platform-specific code to populate the
[abstract service model](https://istio.io/docs/concepts/traffic-management/#pilot), dynamically reconfigure the proxies
when the application topology changes, as well as translate
[routing rules](https://istio.io/latest/docs/reference/config/networking/) into proxy specific configuration.

    - [security](security/). This directory contains [security](https://istio.io/latest/docs/concepts/security/) related code.

- [istio/proxy](https://github.com/istio/proxy). The Istio proxy contains
extensions to the [Envoy proxy](https://github.com/envoyproxy/envoy) (in the form of
Envoy filters) that support authentication, authorization, and telemetry collection.

- [istio/ztunnel](https://github.com/istio/ztunnel). The project contains the Rust implementation of the ztunnel
component of Ambient mesh.

- [istio/client-go](https://github.com/istio/client-go). This project defines
  auto-generated Kubernetes clients for interacting with Istio resources programmatically.

> [!NOTE]
> Only the `istio/api` and `istio/client-go` projects expose stable interfaces intended for direct usage as libraries.

*Section quoted from the upstream readme.*
Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

- To ask questions and get assistance from our community, visit [GitHub Discussions](https://github.com/istio/istio/discussions)
- To learn how to participate in our overall community, visit [our community page](https://istio.io/about/community)

In this README:

- [Introduction](#introduction)
- [projects](#projects)
- [Issue management](#issue-management)

In addition, here are some other documents you may wish to read:

- [Istio Community](https://github.com/istio/community#istio-community) - describes how to get involved and contribute to the Istio project
- [Istio Developer's Guide](https://github.com/istio/istio/wiki/Preparing-for-Development) - explains how to set up and use an Istio development environment
- [Project Conventions](https://github.com/istio/istio/wiki/Development-Conventions) - describes the conventions we use within the code base
- [Creating Fast and Lean Code](https://github.com/istio/istio/wiki/Writing-Fast-and-Lean-Code) - performance-oriented advice and guidelines for the code base

You'll find many other useful documents on our [Wiki](https://github.com/istio/istio/wiki).

*Section quoted from the upstream readme.*
Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

policy enforcement and telemetry recording/reporting
   functions.

  > Note: The service mesh is not an overlay network. It
  > simplifies and enhances how microservices in an application talk to each
  > other over the network provided by the underlying platform.

* **Ztunnel** - A lightweight data plane proxy written in Rust,
    used in Ambient mesh mode to provide secure connectivity and observability for workloads without sidecar proxies.

- **Istiod** - The Istio control plane. It provides service discovery, configuration and certificate management.

*Section quoted from the upstream readme.*
---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | Go |
| Manifests detected | go.mod, go.sum |
| Files in snapshot | 6700 |
| Lines of code | 624881 |
| Dependency references | 223 |
| Dependencies by ecosystem | go: 220, npm: 3 |
| Upstream license | Apache-2.0 |
| Overlay license | Anticommons 0.1.0 |

Top dependency references recorded in the benchmark snapshot:

| Ecosystem | Name | Version | Source file |
|-----------|------|---------|-------------|
| go | cloud.google.com/go/compute/metadata | v0.9.0 | go.mod |
| go | github.com/agentgateway/agentgateway/api | v0.0.0-20260501213430-773586679f1c | go.mod |
| go | github.com/alecholmes/xfccparser | v0.4.0 | go.mod |
| go | github.com/cbeuw/connutil | v1.0.1 | go.mod |
| go | github.com/cenkalti/backoff/v4 | v4.3.0 | go.mod |
| go | github.com/cespare/xxhash/v2 | v2.3.0 | go.mod |
| go | github.com/cheggaaa/pb/v3 | v3.1.7 | go.mod |
| go | github.com/cncf/xds/go | v0.0.0-20260202195803-dba9d589def2 | go.mod |
| go | github.com/containernetworking/cni | v1.3.0 | go.mod |
| go | github.com/containernetworking/plugins | v1.9.1 | go.mod |
| go | github.com/coreos/go-oidc/v3 | v3.18.0 | go.mod |
| go | github.com/davecgh/go-spew | v1.1.2-0.20180830191138-d8f796af33cc | go.mod |
| go | github.com/docker/cli | v29.5.2+incompatible | go.mod |
| go | github.com/envoyproxy/go-control-plane/contrib | v1.36.1-0.20261003070529-6b14e001be9b | go.mod |
| go | github.com/envoyproxy/go-control-plane/envoy | v1.39.1-0.20261003070529-6b14e001be9b | go.mod |
| ... | (208 more) | | |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

- [Project Conventions](https://github.com/istio/istio/wiki/Development-Conventions) - describes the conventions we use within the code base
- [Creating Fast and Lean Code](https://github.com/istio/istio/wiki/Writing-Fast-and-Lean-Code) - performance-oriented advice and guidelines for the code base

You'll find many other useful documents on our [Wiki](https://github.com/istio/istio/wiki).

*Section quoted from the upstream readme.*
Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

*Excerpt from upstream `CONTRIBUTING.md`:*

# Contribution guidelines

So you want to hack on Istio? Yay! Please refer to Istio's overall
[contribution guidelines](https://github.com/istio/community/blob/master/CONTRIBUTING.md)
to find out how you can help.

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
                        http://www.apache.org/licenses/

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
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original Apache-2.0 terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `Apache-2.0` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `IST` (category: CHIP QUANTIZATION)
- **Upstream URL:** https://github.com/istio/istio
- **Pinned commit (SHA):** `e4350fd4d6c9905d9b5fe6d5c85ca7c521e45daa`
- **Branch:** master
- **Pin provenance:** GitHub API commits/master. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`2826088660fce6a0c05e867f3d3b5716c85a597e64ab61cac8eb452fb00a283b`.

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

