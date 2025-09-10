#  The FreeBSD Foundation's *STA Work Package E - Software Bill of Materials*

| Project Name | STF Work Package E - Improve existing, and implement new, tooling and processes for FreeBSD Software Bill of Materials (SBOM)|
| :---- | :---- |
| Comissioning Body | Sovereign Tech Agency |
| Funding Status | Approved on August 26, 2024 |
| Scheduling | April 2025 - December 2025 |
| Project Sponsor | [Ed Maste](https://github.com/emaste) |
| Project Manager | [Alice Sowerby](https://github.com/alice-sowerby) |
| Objectives | Contract wording with STA: </br></br>“Improve existing, and implement new, tooling and processes for FreeBSD Software Bill of Materials (SBOM) <br> 1) Implement tooling to roll up the individual provenance data/markers from across the tree into a higher-level view.<br> 2) Develop tooling to parse/review/inspect the FreeBSD source tree and produce a comprehensive/holistic report to act as a SBOM for the full software stack. <br> 3) Extend pkg to enable this capability for software installed from ports/packages.”|
| Organization goals | SBOMs are becoming an industry standard for improving visibility of the “software supply chain” for open source (and other) codebases. This visibility can enable efforts to :<br> - Improve relationships and support for upstream projects and overall open source ecosystem. <br> - Understand and respond to security risks in the supply chain.  <br> - Understand and manage licence compliance in the supply chain. <br><br> The FreeBSD Project would also benefit from taking a rigorous, structured approach to understand its dependencies/3rd-party components, their ownership and maintenance which an SBOM would help to deliver.<br><br>Additionally, the Foundation has had feedback from Enterprise users (especially downstream commercial users) that they need to have SBOMs for all the parts of their software supply chain(s). This is being driven to a great degree by new regulations in the USA and other regions.<br><br>To meet the needs of users, the SBOM output should meet a widely-used standard and be easily accessible without a human in the loop. To meet the needs of the FreeBSD Project, the solution (tooling and processes developed) needs to have an ongoing (post-project) owner, and be as automated as practical.|
| Output | An SBOM can be produced through CI for any build.<br>An SBOM for each release is produced as a release artifact.<br>Producing SBOMs and managing the process has an owner within the FreeBSD Project.|

## Stakeholder Analysis

R = Responsible, A = Accountable , C = Consulted, I = Informed

* Core - I 
* Source Manager, Port Manager, Package Manager, Security, Release Engineering Teams - A, C, I
* Assigned developer(s) - R
* Alice Sowerby (Project Manager) - R, C, I
* Ed Maste (Technical Sponsor) - R, A, C, I
* Deb Goodkin (Executive Sponsor) - A, I
* Sovereign Tech Agency (Commissioning Body) - A, I

## Scope
| Within Scope| Outside Scope           |
|:------------|:--------------------------|
| Functional Requirements | |
| **Must** <br> Evaluate projects/solutions available in the wider ecosystem (to avoid building a whole new solution) e.g. [Ariadne's pkgconf proposal](https://ariadne.space/2025/02/08/c-sboms-and-how-pkgconf.html). <br> - Ports may be simpler than for src, solutions will need to be different. <br> - See if there is any existing logic for deciding what needs an SBOM when introduced as a new component. Most likely, this is just subdirectories of contrib, sys/contrib and crypto.<br><br> Based on the info gathered in the previous set, propose the target solution for SBOM. production/distribution for FreeBSD.<br><br> Produce an SBOM in CI (e.g. weekly builds). <br> - Find some downstream projects who would consume the generated SBOM and find out what they need to be able to consume it usefully. Use this to inform the solution. <br><br>Produce an SBOM as a release artifact as part of the release process. <br> - Work with the Foundation to obtain advice on the legal implications of an SBOM and what disclaimers should be included. <br><br>SBOM artifact to be provided to the user in a manner that allows it to be  programmatically collected (e.g. at an endpoint). <br><br>Implement tooling to roll up existing data in FreeBSD that can be used to build the SBOM (individual provenance data/markers from across the tree into a higher-level view). This applies in particular to the contributed software in FreeBSD. <br> - Data/markers to be included in the SBOM should be determined by the SBOM standard selected, but could include: contributed software versions, licenses, and other important information. <br> <br> Set out any limitations (decisions made) on what will be done to achieve a useful SBOM, and identify anything out of scope that may be tackled in a later project, or communicated as a “won’t fix”.<br><br> **Should** <br> Engage in other similar efforts in the ecosystem e.g. https://ariadne.space/2025/02/08/c-sboms-and-how-pkgconf.html| **Won’t** <br><br> Not to be retroactively applied to older releases/versions. <br><br>Not to target 1000s of ports.|
| Non-Functional Requirements | |
| - Output to meet some SBOM standard in common use. <br> - SBOM to cover FreeBSD Kernel (src)<br> - SBOM to cover packages installed through pkg.<br> -  SBOMs from key 3rd party packages that are included in official release images0 (perl, python, curl, cloudinit etc ..)| |

## Quick links
[Latest Updates](Updates)

[Meeting Notes](Meeting-Notes)

[Foundation blog about the Sovereign Tech Agency commission](https://freebsdfoundation.org/blog/sovereign-tech-fund-to-invest-e686400-in-freebsd-infrastructure-modernization/)


## Discussion threads
We support using the FreeBSD [mailing lists](https://lists.freebsd.org/) as the community's preferred way to discuss all FreeBSD matters. 
e.g. [FreeBSD Hackers Mailing List](https://lists.freebsd.org/archives/freebsd-hackers/)

## FAQs

### How much is being invested in this work?

The total value of the STA commission is €686,400 to drive improvements in infrastructure, security, regulatory compliance, and developer experience.

### How long is this program due to run?

The overall program will start in August 2024 and end in December 2025.

### How was the scope of the work decided? 

The high-level scope was outlined by the FreeBSD Foundation with input from the community, including key stakeholders identified earlier in this document.

### What exactly is covered in the planned work?   
The scope will be unpacked month by month as we make progress, focusing on where the most high-value functionality can be achieved with the resources and support that we have available. Check out the [Meeting Notes](Meeting-Notes) to see how the work is being discussed over time.

### Who will be doing the work?

The Foundation will be managing staff and a group of contracted FreeBSD developers to work on different functional areas to deliver regular updates on the project goals. 

### How can I share my views on what would make this project better?
If your suggestions are suitable for public discussion, we ask that you start a conversation in the most suitable [FreeBSD mailing list](https://lists.freebsd.org/) or you can reach the Foundation through the usual channels given on the [FreeBSD Foundation Contact Us webpage](https://freebsdfoundation.org/about-us/contact-us/).

### How can I keep up to date with the work in progress and any new releases?

There are several ways to keep yourself in the loop. 

1. Read the [monthly updates](Updates) that are posted into this repo.
2. Seek out the recordings of the Technology Team Updates given at BSD conferences such as BSDCan.
4. Read the quarterly reports on FreeBSD.org
5. Sign up to the FreeBSD Foundation newsletter. All announcements about the program will be included in our updates.

### How is this repo being used by the Foundation for this project?
We are using this repo to capture key project information and updates. We are not using it for source code management. The repo is read-only for the public.