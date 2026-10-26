# [DRAFT] Program Brief and FAQs

## Sovereign Tech Agency FreeBSD investment for 2026

| Program Name | Improvements for Production Quality FreeBSD Enterprise Deployments |
| :---- | :---- |
| Funding Body | [Sovereign Tech Agency](https://www.sovereigntechfund.de/) |
| Funding Status | Approved on October 9, 2026 |
| Program Sponsor | Ed Maste |
| Program Manager | Anne Dickison |
| Objectives | - Upstream FreeBSD support in OpenJDK. Expand bhyve virtualization capabilities. <br /> - Develop production-quality pkgbase deployment and upgrade support. <br /> - Add FreeBSD networking support to Netavark.<br /> -  Research and develop an SBOM solution for FreeBSD.<br /> -  Develop automated and advanced developer tooling.<br /> -  Improve FreeBSD Ports and Package infrastructure.<br /> -  Develop production-quality secure boot support.<br /> -  Develop next-boot and rescue environment support |
| Organization goals | The proposed work addresses fundamental challenges threatening the longevity and independence of FreeBSD and open digital infrastructure in general. The proposed work addresses gaps in areas including virtualization, containers, system upgrades and recovery, Secure Boot, software supply-chain information, package infrastructure, and Java support.  Some of these gaps require users to create their own patches, tools, or workarounds, adding cost and complexity. The work will explore possible approaches, build and test new solutions, and integrate them upstream where appropriate. This improves interoperability and expands where FreeBSD can be a practical option. |

# Quick Links

* FreeBSD Foundation’s project launch blog  
* Monthly updates  
* Sovereign Tech Agency’s project launch announcement

# Work packages

## Work Package A: Upstream FreeBSD Support in OpenJDK

### Why we chose this work

Bringing FreeBSD support upstream will improve Java portability and reduce reliance on a separate FreeBSD patch set. It will also make FreeBSD a better-supported platform within the wider Java ecosystem, giving users more choice in where Java workloads can run.

### What is included

1. Review and curate the FreeBSD patches required to build and run OpenJDK.  
2. Prepare and submit FreeBSD support to the upstream OpenJDK project, and work with maintainers to address review and integration requirements.  
3. Reduce the FreeBSD-specific patch set that must be carried outside the upstream project.

## Work Package B: Expand bhyve Virtualization Capabilities

### Why we chose this work

These capabilities will make bhyve more practical for production and large-scale virtualization. Migration support will give operators more flexibility to move workloads and manage infrastructure with less disruption. Better integration with common management tools will also make bhyve easier to use alongside existing open source virtualization technologies.

### What is included

1. Evaluate relevant improvements from the illumos port of bhyve and integrate appropriate changes into FreeBSD.  
2. Implement guest suspension and offline or warm migration.  
3. Implement live migration of running bhyve guests.  
4. Extend Sylve to improve management of bhyve environments.  
5. Improve bhyve support in libvirt and virt-manager.

## Work Package C: Develop Production-Quality pkgbase Deployment and Upgrade Support

### Why we chose this work

Pkgbase will give organizations a more consistent way to deploy and update the FreeBSD base system using package-management workflows. This is especially important for large deployments, where upgrades need to be automated and recoverable.

### What is included

1. Develop the pkgbase functionality needed for production deployment and system  
2. upgrades.  
3. Develop and improve rollback and recovery workflows.  
4. Improve support for automated system upgrades.  
5. Develop workflows for managing pkgbase upgrades across multiple systems.

## Work Package D: Add FreeBSD Networking Support to Netavark

### Why we chose this work

FreeBSD can run OCI-compatible containers, but networking remains a major missing capability. Adding FreeBSD support to Netavark will close that gap while contributing support to an upstream project used by the broader container ecosystem. This gives developers and operators another platform for running containerized workloads using open standards.

### What is included

1. Implement Rust bindings for FreeBSD's pf firewall.  
2. Integrate the pf binding library into Netavark and produce a FreeBSD port.  
3. Create, update, or integrate an Aardvark-DNS port for FreeBSD.

## Work Package E: Research and Develop an SBOM Solution for FreeBSD

### Why we chose this work

Extending the FreeBSD SBOM solution to support the CycloneDX format will make it accessible to more users. It will also help to establish the SBOM as the backbone for scanning the FreeBSD dependency base for known vulnerabilities logged in centralized vulnerability databases. Updating pkg to support SBOMs will also streamline and simplify this solution, by allowing us to generate or manipulate SBOMs with pkg. Adding support for FreeBSD to PURL will allow adoption of this standardized package locator format within FreeBSD. Creating an SBOM for ports will significantly improve the ability of FreeBSD users to understand their dependencies as required by legislation such as the EU’s Cyber Resilience Act.

### What is included

1. Add CycloneDX support to the SBOM solution  
   1. Implementation upstream in pkgconf  
   2. (Vendor update in FreeBSD)  
   3. Support in FreeBSD’s base system (share/mk/bsd.sbom.mk)  
   4. Additional support for binary hashes in SBOMs (useful for CycloneDX)  
2. 2\. Add FreeBSD support in PURL (Package URL)  
   1. Complete the specification updates (PURL, OSV) in coordination with core, srcmgr, portmgr, secteam, ports-secteam  
   2. Implementation upstream in pkgconf  
   3. Updating the meta-data in FreeBSD (i.e., in the Makefile.sbom files)  
3. 3\. Extend the SBOM for the FreeBSD ports collection  
   1. Generate SBOM files when building ports  
   2. Migrate from VuXML to a common standard  
4. 4\. Make pkg SBOM-aware  
   1. Import pkg into the base system  
   2. Use an SBOM-based vulnerability database instead of VuXML

## Work Package F: Develop Automated and Advanced Developer Tooling

### Why we chose this work

Better developer tooling will make it easier to review and validate changes across a large, integrated operating system codebase. It can also help contributors identify problems earlier and make better use of limited developer time.

### What is included

1. Bottleneck assessment (published report). A written survey of FreeBSD development workflows identifying repeated technical bottlenecks, with data drawn from CI, release artifact and package-build logs, Phabricator/Bugzilla activity, and developer input. Published to the FreeBSD developer community for comment.  
2. Selection and specification. A short design document for each selected intervention: scope, interfaces, hosting/maintenance plan, and acceptance criteria. Selection will use the ranking from deliverable 1 together with the availability of contributors with the relevant expertise.  
3. At least two tools delivered and in production use. Each will be committed to a public repository, documented, and deployed on Project or developmental infrastructure. Candidate tools are listed below. At least two tools will be chosen from this list, or tools of similar scope identified in deliverable 1\.   
   1. Improve integration of ports tests: FreeBSD has over 30,000 third party software packages in its ports collection. Many of those ports include tests, but they are not well integrated into the overall FreeBSD infrastructure. Add support to FreeBSD tools such as Poudriere to execute and report results from tests included in 3rd party software.  
   2. Automated triage of continuous-integration and package-build failures: classify failures by cause (e.g. dependency breakage, flaky test, infrastructure fault), deduplicate, and route to the responsible maintainer.  
   3. Dependency-impact validation for ports changes: given a proposed change, enumerate all dependent ports and test-build them before commit.  
   4. Pre-commit testing of base-system changes: build and run the relevant test suites against a proposed change before it lands in main.  
   5. Automated review assistance: style, lint, and policy checks applied to proposed changes with results posted to the review.  
   6. Production of build artifacts for candidate changes: Given a series of patches to the base system, produce artifacts for installation of new, and or upgrade of existing, FreeBSD deployments, to allow broader testing changes with increased risk or backwards compatibility concerns.  
   7. Reviewer and maintainer routing: Build on existing work to suggest reviewers for an externally submitted patch, flag changes with no maintainer, and track maintainer-timeout deadlines.  
4. Adoption and handover. Documentation for each tool, an announcement and walkthrough for committers, and an identified maintainer or team within the Project for each tool after the funding period ends.

## Work Package G: 

### Why we chose this work

The Ports Collection was not built for current security and compliance expectations. Subpackages reduce installed attack surface, package tiering gets security rebuilds to production users faster, and a more predictable Poudriere enables the reproducible builds and metadata the SBOM work in Work Package E depends on — capabilities the appliance, hosting, and embedded manufacturers shipping FreeBSD-based products now need under the EU Cyber Resilience Act.

### What is included

1. Evaluate priority improvements to the Ports and package-building infrastructure:  
   1. Finalize incomplete work to implement subpackages  
   2. Deploy shared infrastructure for developers to test ports on all supported releases for all tier 1 architectures  
   3. Design a provides/requires system for FreeBSD ports  
2. Develop selected improvements in areas such as subpackages, Poudriere, or package tiering.  
3. Integrate completed improvements into the appropriate FreeBSD infrastructure.

## Work Package H: Develop Production-Quality Secure Boot Support

### Why we chose this work

Secure Boot is increasingly expected in modern infrastructure. In some environments, it is needed to verify that boot software has not been tampered with. In others, it is required by the hardware platform itself.

FreeBSD currently has limited support for these use cases. Some configurations are possible, but they require significant manual work. Other hardware requirements cannot currently be addressed at all.

Production-quality Secure Boot support would improve system security and remove a barrier to using FreeBSD on modern hardware. It would also give organizations another open platform that can meet current hardware trust requirements.

### What is included

1. Advancements in support of boot shim support.  
2. Loader support for secureboot policies  
3. Kernel support for secureboot policies.  
4. Signing of relevant boot components.  
5. Development of a maintainable signing and validation process.

## Work Package I: Develop Next-Boot and Rescue Environment Support

### Why we chose this work

Reliable recovery is important for systems that cannot easily be accessed in person. Next- boot and automatic fallback capabilities will allow operators to make changes with less risk of leaving remote systems inaccessible. The work also complements pkgbase by providing recovery options when automated upgrades do not succeed.

### What is included

1. Improve loader next-boot support.  
2. Allow an alternate boot or rescue environment to be selected for the next startup.  
3. Detect repeated failed boots.  
4. Automatically fall back to a known-good or rescue environment after a defined number of failures.  
5. Improve recovery options for remotely managed and self-hosted FreeBSD systems.

# FAQs

### Why is the Sovereign Tech Agency interested in FreeBSD?

The Sovereign Tech Agency has a [mission](https://www.sovereigntechfund.de/mission/) to support digital sovereignty in digital infrastructure through supporting open source projects.

FreeBSD is an excellent candidate for helping the STA achieve its mission.  
It is a project that supports digital sovereignty through offering infrastructure diversity. It has an independent governance model and self-hosted development and build systems.

FreeBSD provides superior security, performance, and stability in a single production-ready package that is ideal for systems that demand freedom of use and long-term reliability. At the heart of FreeBSD’s philosophy is a steadfast commitment to the BSD license, which reflects the project’s foundational principles of freedom and open innovation. FreeBSD’s development model is driven by the spirit of collaboration inherited from Berkeley’s BSD. Upstream contributions made by the community impact the entire system, from the kernel to utilities and documentation, resulting in a unified approach where every enhancement benefits the entire ecosystem.

### How did the Foundation decide on these work packages?

We have proposed work packages that meet both FreeBSD goals and STA’s mission.  
The FreeBSD Foundation’s application was informed by extensive input from across the project, to include leading developers, Core Team, and users.

### How does this investment fit in with other funding we have received?

Donations from FreeBSD users \- both individual and corporate \- have been largely sufficient to fund the priority needs of the Foundation over its 25-year history. However, new and expanding needs, in particular the significant expense associated with security, bring near-term costs that exceed our donations. Seeking targeted investment such as this helps to bridge the gap.

### How much money has been invested?

The Sovereign Tech Agency is commissioning work totaling 464,160 EUR.

### When will work start and end?

The work will begin in October 2026 and is due to end in January 2027\.

### How will the money be spent?

Each workstream will be fully funded, and the Foundation will use existing staff and contractors to carry out the work.

### How can I apply for the work?

All work is already fully resourced through existing contractors and/or staff. If you are interested in working with the Foundation in the future, please visit [https\://freebsdfoundation.org/open-positions/](https://freebsdfoundation.org/open-positions/). We are always pleased to meet new people who have relevant FreeBSD experience and who would like to register their interest in working with the Foundation. You can drop us an introduction at [proposals@freebsdfoundation.org](mailto:proposals@freebsdfoundation.org). 

### How can I ask questions or provide feedback?

If your suggestions are suitable for public discussion, we ask that you start a conversation in the most suitable FreeBSD mailing list or you can reach the Foundation through the usual channels [https\://freebsdfoundation.org/about-us/contact-us/](https://freebsdfoundation.org/about-us/contact-us/)

### How can I stay up to date with the work?

There are several ways to keep yourself in the loop.

1. Read the monthly updates that are posted into this repo.  
2. Seek out the recordings of the Technology Team Updates given at BSD conferences such as BSDCan.  
3. Read the quarterly reports on FreeBSD.org  
4. Sign up to the FreeBSD Foundation newsletter. All announcements about the program will be included in our updates.

