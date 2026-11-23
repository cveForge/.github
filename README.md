<!-- ═══════════════════════════ HEADER ═══════════════════════════ -->

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/cveForge/.github/main/assets/readme-banner-dark-3200x800@2x.png">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/cveForge/.github/main/assets/readme-banner-light-3200x800@2x.png">
    <img src="https://raw.githubusercontent.com/cveForge/.github/main/assets/readme-banner-dark-3200x800@2x.png" alt="cveForge — open-source security research" width="100%">
  </picture>
</p>

<p align="center">
  <a href="https://github.com/cveForge">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=24&duration=3200&pause=900&color=F97316&center=true&vCenter=true&multiline=false&repeat=true&width=720&height=50&lines=Forging+tools+for+defenders.;Vulnerability+research+%E2%80%A2+CVE+analysis.;Reverse+engineering+%E2%80%A2+Binary+analysis.;Detection+engineering+%E2%80%A2+Hardening.;Open+source.+Built+in+Rust." alt="cveForge">
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/mission-defensive%20security-F97316?style=flat-square&labelColor=0D1117">
  <img src="https://img.shields.io/badge/license-MIT%20%7C%20Apache--2.0-F97316?style=flat-square&labelColor=0D1117">
  <img src="https://img.shields.io/badge/disclosure-coordinated-F97316?style=flat-square&labelColor=0D1117">
  <img src="https://img.shields.io/github/followers/cveForge?style=flat-square&color=F97316&labelColor=0D1117&label=followers">
</p>

<p align="center">
  <a href="#-who-we-are">About</a> •
  <a href="#-what-we-do">What we do</a> •
  <a href="#-how-we-work">How we work</a> •
  <a href="#-disclosure-policy">Disclosure</a> •
  <a href="#-engineering-standards">Standards</a> •
  <a href="#-contributing">Contributing</a> •
  <a href="#-contact">Contact</a>
</p>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/fire.png" width="100%">

<!-- ═══════════════════════════ ABOUT ═══════════════════════════ -->

## 🔥 Who we are

**cveForge** is an independent, open-source security research organization.
We study how software breaks — and turn that knowledge into tools that help defenders find, understand and fix vulnerabilities **before** they are exploited.

Every line of code we publish is written with one question in mind:

> ***Does this make the defender's job faster, clearer or safer?***

If the answer is no, it doesn't ship.

<table>
<tr>
<td width="33%" valign="top">

### 🛡️ Defensive first
Our tooling is designed for blue teams, product security engineers, SOC analysts and independent researchers. Detection, triage and remediation come first.

</td>
<td width="33%" valign="top">

### ⚙️ Engineered in Rust
Memory-safe by default, fast without compromise. Security tools should not be the weakest link in your stack.

</td>
<td width="33%" valign="top">

### 🌐 Open by design
Permissive licenses, transparent research, reproducible results. Knowledge locked away doesn't protect anyone.

</td>
</tr>
</table>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/fire.png" width="100%">

<!-- ═══════════════════════════ FOCUS AREAS ═══════════════════════════ -->

## 🎯 What we do

<table>
<tr>
<td width="50%" valign="top">

#### 🔍 Vulnerability Research
Root-cause analysis of published CVEs, variant hunting across codebases and patch-diffing to understand what was actually fixed — and what wasn't.

#### 🧬 Reverse Engineering
Static and dynamic analysis of binaries, firmware and bytecode. Disassembly, decompilation and control-flow recovery tooling built for speed.

#### 🧩 Deobfuscation & Code Analysis
Unpacking and normalizing obfuscated code across multiple languages so analysts can read what software *really* does.

</td>
<td width="50%" valign="top">

#### 🦠 Malware Analysis
Behavioral and structural analysis of malicious samples, IOC extraction and signature development for detection pipelines.

#### 🌍 Network & Infrastructure Security
Routing security research, traffic inspection, DDoS mitigation and edge-defense engineering.

#### 🧪 Detection Engineering
Turning research into practical detections: rules, signatures, scanners and hardening guides that defenders can deploy today.

</td>
</tr>
</table>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/fire.png" width="100%">

<!-- ═══════════════════════════ WORKFLOW ═══════════════════════════ -->

## 🔁 How we work

Every research effort follows the same forge cycle — from raw finding to hardened defense:

```mermaid
flowchart LR
    A["🔎 Discover<br/><sub>audit · fuzz · patch-diff</sub>"] --> B["🧪 Analyze<br/><sub>root cause · impact</sub>"]
    B --> C["📨 Disclose<br/><sub>coordinated with vendor</sub>"]
    C --> D["🛠️ Forge<br/><sub>detections · tooling</sub>"]
    D --> E["📚 Publish<br/><sub>advisory · write-up</sub>"]
    E -.-> A

    style A fill:#1a1a1a,stroke:#F97316,color:#fff
    style B fill:#1a1a1a,stroke:#F97316,color:#fff
    style C fill:#1a1a1a,stroke:#F97316,color:#fff
    style D fill:#1a1a1a,stroke:#F97316,color:#fff
    style E fill:#F97316,stroke:#F97316,color:#000
```

| Stage | What happens | Output |
|:--|:--|:--|
| **Discover** | Code audits, fuzzing campaigns, patch diffing, threat-intel review | Candidate findings |
| **Analyze** | Root-cause analysis, exploitability and impact assessment, severity scoring | Technical report |
| **Disclose** | Private notification to the affected vendor or maintainer | Coordinated timeline |
| **Forge** | Build detection rules, scanners and mitigations around the finding | Open-source tooling |
| **Publish** | Advisory and technical write-up after a fix is available | Public knowledge |

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/fire.png" width="100%">

<!-- ═══════════════════════════ DISCLOSURE ═══════════════════════════ -->

## 📨 Disclosure policy

We follow **Coordinated Vulnerability Disclosure (CVD)**. Our default process:

- 🔒 **Private first** — findings are reported privately to the vendor or maintainer before anything goes public.
- ⏳ **90-day window** — the standard deadline for a fix, extendable when the vendor is actively working in good faith.
- 🤝 **Collaboration** — we share reproduction details, analysis and suggested mitigations with the affected party.
- 📢 **Publish after fix** — advisories and write-ups are released once users have a reasonable chance to patch.
- 🚫 **No weaponization** — we never publish working exploits for unpatched vulnerabilities.

> [!IMPORTANT]
> Found a vulnerability **in one of our own projects**? Please don't open a public issue.
> Use **GitHub Private Vulnerability Reporting** on the affected repository (Security → *Report a vulnerability*).

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/fire.png" width="100%">

<!-- ═══════════════════════════ STACK ═══════════════════════════ -->

## 🧰 Toolchain

<p align="center">
  <img src="https://skillicons.dev/icons?i=rust,go,wasm,c,cpp,py,ts,linux,docker,githubactions&theme=dark&perline=10" alt="Tech stack">
</p>

<div align="center">

| Layer | Technologies |
|:--:|:--|
| **Core engines** | Rust · Go |
| **Low level** | C / C++ · eBPF · x86-64 / ARM64 |
| **Portable** | WebAssembly · TypeScript |
| **Research & glue** | Python |
| **Infrastructure** | Linux · Docker · GitHub Actions |

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/fire.png" width="100%">

<!-- ═══════════════════════════ STANDARDS ═══════════════════════════ -->

## 📐 Engineering standards

Security tools hold a privileged position — they run with high access, on sensitive data, inside critical environments. We hold ourselves to a high bar:

<details open>
<summary><b>🦀 Code quality</b></summary>
<br>

- Memory-safe languages by default; `unsafe` blocks are minimized, isolated and documented
- `clippy` pedantic + `rustfmt` enforced in CI
- Fuzzing for every parser that handles untrusted input
- Reproducible builds wherever possible

</details>

<details>
<summary><b>🔐 Supply chain</b></summary>
<br>

- Dependencies audited with `cargo audit` / `cargo deny`
- Minimal dependency trees — fewer crates, smaller attack surface
- Signed releases and published checksums
- Dependabot and security advisories enabled on every repository

</details>

<details>
<summary><b>📖 Documentation</b></summary>
<br>

- Every tool ships with a clear README, usage examples and threat model
- Intended use and limitations are stated explicitly
- Changelogs follow [Keep a Changelog](https://keepachangelog.com)
- Versioning follows [SemVer](https://semver.org)

</details>

<details>
<summary><b>⚖️ Responsible use</b></summary>
<br>

- Tools are intended for **authorized** security testing, research and defense only
- We do not accept contributions designed to target systems without authorization
- Use of our software must comply with applicable laws and regulations

</details>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/fire.png" width="100%">

<!-- ═══════════════════════════ CONTRIBUTING ═══════════════════════════ -->

## 🤝 Contributing

We welcome researchers, engineers and curious minds. There are many ways to help:

| | Way to contribute | How |
|:--:|:--|:--|
| 🐛 | **Report bugs** | Open an issue with steps to reproduce |
| 💡 | **Suggest features** | Start a discussion describing the use case |
| 🧑‍💻 | **Submit code** | Fork → branch → PR with tests |
| 📝 | **Improve docs** | Typos, examples and guides are always welcome |
| 🔬 | **Share research** | Detection ideas, test samples, edge cases |

**Before your first PR:**
1. Read the repository's `CONTRIBUTING.md`
2. Make sure `cargo fmt`, `cargo clippy` and `cargo test` pass
3. Keep pull requests focused — one change per PR
4. Be respectful — our Code of Conduct applies everywhere

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/fire.png" width="100%">

<!-- ═══════════════════════════ CONTACT ═══════════════════════════ -->

## 📬 Contact

<div align="center">

| Purpose | Channel |
|:--|:--|
| 🔐 **Security reports** | GitHub Private Vulnerability Reporting on the affected repo |
| 💬 **Questions & ideas** | GitHub Discussions |
| 🐞 **Bugs** | GitHub Issues on the relevant repository |

</div>

<!-- ═══════════════════════════ FOOTER ═══════════════════════════ -->

<br>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/cveForge/.github/main/assets/cveforge-mark-orange.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/cveForge/.github/main/assets/cveforge-mark-orange.svg">
    <img src="https://raw.githubusercontent.com/cveForge/.github/main/assets/cveforge-mark-orange.svg" alt="cveForge mark" height="72">
  </picture>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/cveForge/.github/main/assets/cveforge-wordmark-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/cveForge/.github/main/assets/cveforge-wordmark-light.svg">
    <img src="https://raw.githubusercontent.com/cveForge/.github/main/assets/cveforge-wordmark-dark.svg" alt="cveForge" height="36">
  </picture>
</p>

<p align="center">
  <sub><i>Every vulnerability understood is one less weapon in the wrong hands.</i></sub>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:7C2D12,100:F97316&height=120&section=footer" width="100%">
</p>
