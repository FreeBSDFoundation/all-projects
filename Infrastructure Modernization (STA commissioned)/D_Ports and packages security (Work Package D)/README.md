#  The FreeBSD Foundation's *STA Work Package D - Ports and Packages Security*

| Project Name | STF Work Package D - Modernize and extend security controls in the FreeBSD Ports and Package Collection |
| :---- | :---- |
| Comissioning Body | Sovereign Tech Agency |
| Funding Status | Approved on August 26, 2024 |
| Scheduling | April 2025 - December 2025 |
| Project Sponsor | [Ed Maste](https://github.com/emaste) |
| Project Manager | [Alice Sowerby](https://github.com/alice-sowerby) |
| Objectives | Contract wording with STA: </br></br>“Modernize and extend security controls in the FreeBSD Ports and Package Collection: <br> 1) Migrate from our VuXML Vulnerability Database to OSV (or other agreed format). <br> 2) Develop a package audit backend and server to reliably fetch vulnerability data from global agency databases in any format (JSON - NIST) and produce insight. <br> 3) Improve CI tooling for FreeBSD Ports.”|
| Organization goals | The goal is that FreeBSD will consume and contribute to Vulnerability Databases using industry-standard format. <br><br> Having CI in ports will allow us to more quickly release updates, which supports a strong security posture for addressing vulnerabilities.|
| Output | All existing and future FreeBSD Ports vulnerabilities will be captured and managed in OSV (or agreed) format, and made available to automated processes within FreeBSD and for 3rd-party entities. <br><br> A CI infrastructure will be in place for Ports, creating using industry-standard practices. |

## Stakeholder Analysis

R = Responsible, A = Accountable , C = Consulted, I = Informed

* Core - I 
* Source Manager, Port Manager, Package Manager, Security Teams - A, C, I
* Assigned developer(s) - R
* Alice Sowerby (Project Manager) - R, C, I
* Ed Maste (Technical Sponsor) - R, A, C, I
* Deb Goodkin (Executive Sponsor) - A, I
* Sovereign Tech Agency (Commissioning Body) - A, I

## Scope
| Within Scope| Outside Scope           |
|:------------|:--------------------------|
| Functional Requirements | |
| **Must** <br> Select a new format for the Vulnerability Database. Whether this is OSV or another format to be determined in the course of the work. <br><br>   Set up database instance (2+ for security purposes). <br> <br> Transform and migrate data between VuXML database and new database.<br> -  Keep separate the transition between DBs and the transition of the tools that use it. (I.e. The DB transition is completed first before tools are changed.) <br> <br> Support for the new format in FreeBSD’s package manager pkg(8).<br> <br> Participate in upstream working groups e.g. OSV as needed to ensure that our work is aligned and integrated where necessary or beneficial. <br> <br> Propose a solution architecture for the combining and presenting to the user on demand: FreeBSD package vulnerability data and data from 3rd parties relating to combined package sets.<br> - Remove the burden of collecting this manually for pkg (make it automated)<br> - Pkg should be able to overwrite/augment data in the ports tree that we import from 3rd party. <br> <br> FreeBSD-specific build and test targets (e.g. portlint)<br> - This implicates 2 types of test. 1) built in test suite that comes with some ports. 2) FreeBSD test targets that validate metadata and so on. <br> - We already have a test framework that can do this, it’s not activated by default. Would mainly be a documentation task to capture how to set it up to achieve this. <br> - Consider creating a CI pipeline to provide a pre-commit (locally) and pre-merge (PR).<br><br> Integrate existing third-party software test targets with FreeBSD ports build infrastructure <br> - This already exists and needs more documentation. <br> - This should be included in the CI pipeline mentioned in the previous bullet point. <br><br> Provide both:<br> - Pre-commit/PR build and test.<br> - Scheduled regular CI tests.<br> - To help reduce the downtime created by long periods without testing that lead to large, complex changes being tested in one go. <br> - A full build should be tested every time a change is made. (Continuous testing)<br> <br> **Could** <br> Make artifacts built by CI tasks available for ad-hoc user/smoke testing.| **Won’t** <br> Add tests to third-party ports|
| Non-Functional Requirements | |
| * Use an industry standard for a vulnerability DB. <br> - Could be all done outside the cluster (cfr. Debian.net )<br> - Ports CI can be done on VMs/external provider. For development we can use donated infrastructure.  <br> - We would want flexibility to update VMs with different snapshots/versions of FreeBSD and no need for root access. <br> - We need a path to hosting this in the long term for the community. <br> - It will be beneficial to create an introduction to IAC for the FreeBSD project e.g. Terraform, Ansible| |

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