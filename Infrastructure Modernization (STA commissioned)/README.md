# Program Brief and FAQs

## Sovereign Tech Agency FreeBSD investment for 2024-25

| Program Name | Infrastructure Modernization |
| :---- | :---- |
| Funding Body | [Sovereign Tech Agency](https://www.sovereigntechfund.de/) |
| Funding Status | Approved on August 19, 2024 |
| Program Sponsor | [Ed Maste](mailto:emaste@freebsdfoundation.org) |
| Program Manager | [Alice Sowerby](mailto:alice@freebsdfoundation.org) |
| Objectives | Uplevel the hygiene and security tooling of base and ports and packages. Modernize the project’s infrastructure to accelerate development cycles. Improve build security. Streamline the onboarding of new developers. |
| Organization goals | Support sustainable ongoing development, improvement, and maintenance of the project. Boost global technological diversity.  Improve the project’s security and resilience.  |
| Output | Work Package A: Pay down technical debt and implement tools and processes to keep it low. Work Package B: Improve tooling and processes to support Zero Trust Builds of FreeBSD. Work Package C: Improve CI/CD automation to streamline software delivery and operations for new and existing software. Work Package D: Modernize and extend security controls in the FreeBSD Ports and Package Collection. Work Package E: Improve existing, and implement new tooling and processes for FreeBSD Software Bill of Materials (SBOM).  |

# Work packages

## Work Package A: Pay down technical debt and implement tools and processes to keep it low

Perform bug triage and remediation, document patches and fixes, develop a comprehensive vulnerability management program, and assess and implement vulnerability management tools and technologies.  

Duration: 5 months  
Scheduling: Aug 2024 \- Dec 2024  
Hours: 880

## Work Package B: Improve tooling and processes to support Zero Trust Builds of FreeBSD

Extend the current components to enable the project to build release artifacts (package sets, ISO images, etc.) without requiring any special privilege. This would include avoiding any use of superuser privilege during the FreeBSD builds.

Reproducible builds will allow external parties to produce and confirm bit-identical artifacts and will offer infrastructure to verify the reproducibility, along with binary transparency logging.

Duration: 8 months  
Scheduling: January 2025 \- August 2025  
Hours: 1408

## Work Package C: Improve CI/CD automation to streamline software delivery and operations for new and existing software 

Modernized CI/CD will help the FreeBSD development community reduce lead time, reduce costs, increase reliability and security, enhance quality, and streamline the accurate collection and display of metrics. 

This work package will modernize and securitize the existing CI/CD system and extend it to cover the third party packages in the FreeBSD Ports Collection. There is currently no organized, formal CI system in place for Ports and this can present a potential cyber attack vector   
This work is important because reducing developer friction is key to both improving development security and to onboarding new, and retaining existing, developers.

Duration: 6 months  
Scheduling: January 2025 \- June 2025  
Hours: 1056

## Work Package D: Modernize and extend security controls in the FreeBSD Ports and Package Collection

* Migrate from our VuXML Vulnerability Database to OSV or similar contemporary format.  
* Develop a package audit backend and server to reliably fetch vulnerability data from global agency databases in any format (JSON \- NIST) and produce insight.   
* Improve CI tooling for FreeBSD Ports.

Duration: 5 months  
Scheduling: March 2025 \- July 2025  
Hours: 880

## Work Package E: Improve existing, and implement new, tooling and processes for FreeBSD Software Bill of Materials (SBOM)

Many of the primitives needed for SBOM are already present in FreeBSD. This project will implement tooling to roll up the individual provenance data/markers from across the tree into a higher-level view. This applies in particular to the contributed software in FreeBSD. Today the project lacks tooling to indicate contributed software versions, licenses, and other important information. We will develop tooling to parse/review/inspect the FreeBSD source tree and produce a comprehensive/holistic report to act as a SBOM for the full software stack. We will also extend pkg to enable this capability for software installed from ports/packages. 

Duration: 6 months  
Scheduling: April 2025 \- September 2025  
Hours: 1056

# 

# FAQs

### Why is the Sovereign Tech Agency interested in FreeBSD? 

The Sovereign Tech Agency has a [mission](https://www.sovereigntechfund.de/mission/) to support digital sovereignty in digital infrastructure through supporting open source projects. 

FreeBSD is an excellent candidate for helping the STA achieve its mission. 

It is a project that supports digital sovereignty through offering infrastructure diversity. It has an independent governance model and self-hosted development and build systems. 

FreeBSD provides superior security, performance, and stability in a single production-ready package that is ideal for systems that demand freedom of use and long-term reliability. At the heart of FreeBSD’s philosophy is a steadfast commitment to the BSD license, which reflects the project’s foundational principles of freedom and open innovation. FreeBSD’s development model is driven by the spirit of collaboration inherited from Berkeley’s BSD. Upstream contributions made by the community impact the entire system, from the kernel to utilities and documentation, resulting in a unified approach where every enhancement benefits the entire ecosystem.

### How did the Foundation decide on these work packages? 

We have proposed work packages that meet both FreeBSD goals and STA’s mission. 

The FreeBSD Foundation’s application was informed by extensive input from across the project, to include leading developers, Core Team, and users.

FreeBSD’s development and build systems are all self-hosted, an unambiguous expression of our commitment to freedom and digital sovereignty. While our commitment to this approach is unwavering, it brings an increased maintenance burden that has resulted in prolonging the life of build and CI/CD systems that work, but are increasingly behind the hosted state of the art. In order to continue attracting and retaining developers \- the lifeblood of any open source community \- and adhere to emerging security requirements, it is critical that we invest in the software development infrastructure in order to offer a frictionless developer experience on par with hosted platforms with which developers are accustomed. 

### How does this investment fit in with other funding we have received? 

Donations from FreeBSD users \- both individual and corporate \- have been largely sufficient to fund the priority needs of the Foundation over its 25-year history. However, new and expanding needs, in particular the significant expense associated with security, bring near-term costs that exceed our donations. The Foundation has spent more than it has taken in the last two years. The STA investment, alongside the 2024 Alpha-Omega grant, will help fill this near-term gap. 

### How much money has been invested?

The Sovereign Tech Agency is commissioning work totaling 686,400EUR. 

### When will work start?

August 2024

### How will the money be spent? 

Each workstream will be fully funded, and the Foundation will use existing staff and contractors to carry out the work, and where additional resources are needed, it will publish job listings for the work.

### How can I apply for the work?

For projects that require contractors, the Foundation anticipates engaging with existing Committers and Contributors by default through an open application consistent with established Foundation grant processes. Ed Maste will make contractor elections. 

The Foundation will announce contracts in due course, and they will be visible at [https://freebsdfoundation.org/open-positions/](https://freebsdfoundation.org/open-positions/)

### How can I ask questions or provide feedback?

If your suggestions are suitable for public discussion, we ask that you start a conversation in the most suitable FreeBSD mailing list or you can reach the Foundation through the usual channels https://freebsdfoundation.org/about-us/contact-us/

### How can I stay up to date with the work?

There are several ways to keep yourself in the loop.

1. Read the monthly updates that are posted into this repo.  
2. Seek out the recordings of the Technology Team Updates given at BSD conferences such as BSDCan.  
3. Read the quarterly reports on FreeBSD.org  
4. Sign up to the FreeBSD Foundation newsletter. All announcements about the program will be included in our updates.

