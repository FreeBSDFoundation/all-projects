#  The FreeBSD Foundation's *STA Work Package B - Zero-trust Builds Project*

| Project Name | STA Work Package B - Improve tooling and processes to support Zero Trust Builds of FreeBSD |
| :---- | :---- |
| Comissioning Body | Sovereign Tech Agency |
| Funding Status | Approved on August 26, 2024 |
| Scheduling | January 2025 - December 2025 |
| Project Sponsor | [Ed Maste](https://github.com/emaste) |
| Project Manager | [Alice Sowerby](https://github.com/alice-sowerby) |
| Objectives | Contract wording with STA: </br></br>“Extend the current components to enable the project to build release artifacts (package sets, ISO images, etc.) without requiring any special privilege.” |
| Organization goals | Updated build process must deliver: <br><br> **Transparency** <br>Build trust with the users of the project by demonstrating that anyone can build the source without requiring special privilege and giving the means to conduct builds for themselves on the scale that the FreeBSD Project does. <br><br>**Security and Best practices.** <br> Removing the need for special privileges when building the FreeBSD from source means that anyone can do it and therefore verify the origin of their binary. Moving towards more fully adopting principles such as: <br><br> - Working in the open <br> - Complete documentation <br> - Principle of least privilege. |
| Output | Anyone can build FreeBSD source without privilege. Complete documentation of the process is made publicly available. |

## Stakeholder Analysis

R = Responsible, A = Accountable , C = Consulted, I = Informed

* Core - I 
* Source Manager, Release Engineering Teams - A, C, I
* Security Team - C, I
* Assigned developer(s) - R
* Alice Sowerby (Project Manager) - R, C, I
* Ed Maste (Technical Sponsor) - R, A, C, I
* Deb Goodkin (Executive Sponsor) - A, I
* Sovereign Tech Agency (Commissioning Body) - A, I

## Scope
| Within Scope| Outside Scope           |
|:------------|:--------------------------|
| Functional Requirements | |
| **Must** <br> - Standardize all source release build cases using no-root for creation of release artifacts.<br> - Formalize and document make world and release.sh in the context of providing joined-up documentation for a user who wants to understand  reproducible builds and directions on how to do it.  (Some documentation already exists but is not necessarily up to date.) <br> <br> **Should** <br> - Address dependencies such as unprivileged chroot, post-installs in package installation on images, and ZFS mounts <br> - Remove privilege from orchestration tooling e.g. Thermite (build orchestration engine). This would allow users to reproduce builds more easily. <br> - Move build scripts into the public domain. <br><br> **Could** <br> - Environment Standardization: Using tools to create a consistent build environment. <br> - Use enclaves for building (VM inside VM) which is available on various cloud providers. <br> - Build VM images. Inc. disk images for clouds. <br> - Src to build reproducibly <br> - Ports to build reproducibly <br> - CI to verify reproducibility <br> - Documentation to allow 3rd parties to confirm reproducibility|**Won’t** <br> - Make changes to Freebsd-update. <br> - Apply to existing major release branches (14.x and lower). <br> - Move to using a very minimal version of pkg in the base system. <br> - Produce a launchable cloud image. Provide cloud image upload scripts.| 
| Non-Functional Requirements | |
| **Must** <br> - Applies to Main dev branch, 15+ <br> - Full test coverage (unit, integration) <br> - Quality, end to end documentation. <br> - This work applies to base system, ports, packages, release artifacts, etc. – a matrix of deliverables and functional areas.
 | |

## Quick links
[Latest Updates](Updates)

[Meeting Notes](Meeting%20Notes)

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
