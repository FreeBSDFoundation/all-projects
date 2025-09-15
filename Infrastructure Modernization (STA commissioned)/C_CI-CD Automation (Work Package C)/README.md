#  The FreeBSD Foundation's *STA Work Package C - CI/CD automation*

| Project Name | STA Work Package C - Improve CI/CD automation to streamline software delivery and operations for new and existing software |
| :---- | :---- |
| Comissioning Body | Sovereign Tech Agency |
| Funding Status | Approved on August 26, 2024 |
| Scheduling | January 2025 - December 2025 |
| Project Sponsor | [Ed Maste](https://github.com/emaste) |
| Project Manager | [Alice Sowerby](https://github.com/alice-sowerby) |
| Objectives | Contract wording with STA: </br></br>“Modernize and securitize the existing CI/CD system and extend it to cover the third party packages in the FreeBSD Ports Collection.”|
| Organization goals | Efficiency, maintainability, and better developer experience: <br><br> - Reduce developer friction for maintainers and committers to improve developer experience, recruitment and retention. <br> - Reduce lead time, reduce costs, increase reliability and security, enhance quality, and streamline the accurate collection and display of metrics. <br> - Improve maintainability, quality, and security of the third party packages in the FreeBSD Ports Collection by extending CI to cover them. |
| Output | A modern CI system that covers base system, ports, and documentation repositories and can be used by developers and contributors across the development lifecycle. Meets standards set out in [FLOSS Best Practices Criteria (All Levels)](https://www.bestpractices.dev/en/criteria)  |

## Stakeholder Analysis

R = Responsible, A = Accountable , C = Consulted, I = Informed

* Core - I 
* Source Manager, Port Manager, Documentation Engineering, Cluster Admin, Release Engineering Teams - A, C, I
* Assigned developer(s) - R
* Alice Sowerby (Project Manager) - R, C, I
* Ed Maste (Technical Sponsor) - R, A, C, I
* Deb Goodkin (Executive Sponsor) - A, I
* Sovereign Tech Agency (Commissioning Body) - A, I

## Scope
| Within Scope| Outside Scope           |
|:------------|:--------------------------|
| Functional Requirements | |
| **Must** <br> Improve quality of incoming commits by: <br> - Providing system-agnostic tooling and documentation so that maintainers and developers can run CI without requiring a 3rd-party service. <br> - Running pre-merge CI on proposed submissions (e.g. Pull Requests)<br> - Capturing metadata about environments in which tests have been run, allowing them to be reproduced to assist with bug remediation. (The specific aspects of the environment it was tested in that would be needed to allow the bug to be reproduced. E.g. is it in a jail, parallel test runs, non-default sysctls.)<br><br>  Extend CI to the Ports tree.<br><br> Improve understanding and management of CI security by developing a threat model and assessing risks. <br><br>  Develop a method for managing CI proactively including keeping tooling up-to-date and patched. <br><br> **Should** <br> - CI can be run using popular 3rd-party services. <br> - Updating the tests to include standard linters and other relevant automated analysis tools. <br> - Have a good way to manage test cases and the results, e.g. Disable (skip in the CI env) failing cases is already ack’d. and have a ticket tracking, and examine the history of the test cases to easily find out the flakey tests (Jenkins already has it but not very efficient) <br><br>**Could**  <br> Extend the use of branches to isolate changes that allow for more granular debugging.| - Fixing test case bugs which are not directly related to the CI system. <br> - Fixing issues in the software being tested (i.e. failing results from a successful CI run). <br> - Auditing CI for vulnerabilities against the threat model. |
| Non-Functional Requirements | |
|  - Use documentation tree as early adopter / “guinea pig” to prove out any new CI tooling/processes. <br> - Meet https://www.bestpractices.dev/en/criteria  standard <br> - (Must) Support Tier-1 CPU architectures. <br> - (should) Should support Tier-2 architectures.| |

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
