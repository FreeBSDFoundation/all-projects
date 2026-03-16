# Project Brief and FAQs

# Cyber Resilience Act readiness investment for 2026

| Project Name | Cyber Resilience Act Readiness |
| :---- | :---- |
| Funding Body | FreeBSD Foundation |
| Funding Status | Approved on January 01, 2026 |
| Project Sponsor | Deb Goodkin |
| Project Manager | Alice Sowerby |
| Project Goals | **Primary Goal**  <br/>The goal of the project is to ensure that the FreeBSD Foundation, the Project, and the Community are aware of, and actively engaged in, preparing for the CRA so that: <br/><br/> - The Foundation meets its legal obligations as an OSS project steward. The Project can benefit from any new opportunities to receive support from manufacturers. <br/> - The Project is protected from disruption by manufacturers seeking to meet CRA regulations.<br/> - The Community does not experience any reduction in contributions caused by contributors mistakenly thinking they have a legal liability under the CRA. <br/><br/>**Goal limitations**  <br/> Based on current funding, we propose to limit the following goals to only what is essential for achieving the primary goals above: <br/><br/> - Delivering CRA educational activities for the community. <br/> - Actively engaging with upstream/downstream OSS projects. <br/> - Engaging in EU policy development.  <br/> - Gathering quantitative information about effectiveness of work done.  |
| Outcomes | 8 key outcomes fall into 3 categories: <br/><br/>**Foundation readiness** <br/> 1) Compliance as a steward. <br/> 2) Financial/material support from manufacturers.<br/><br/> **Project readiness** <br/> 3) Clear understanding of potential types of critical CRA-related scenarios. <br/> 4) Updated processes and staffing required to cope with above scenarios. <br/> 5) A functional SBOM toolchain. <br/><br/>**Community readiness** <br/> 6) A documented guide to the CRA and how it affects the FreeBSD Project and contributors. <br/> 7) A mechanism for FreeBSD community engagement in EU policymaking. <br/> 8) A public record of work the Foundation is doing on CRA readiness. |

>[!Note]
>A note on the scope of the project.
>
>The CRA is a new piece of legislation and the real-world implementation, best practice, and other implications are constantly evolving.
>Therefore, you should expect to see the scope of this project adapt over time as our understanding develops.

# Quick links
* [Project launch blog post](https://freebsdfoundation.org/blog/getting-ready-for-the-cyber-resilience-act/)
* [Monthly updates](monthly-updates/)
* [Open Consultations and Community Initiatives](legislative-engagement/requests-for-input.md) 

# Workstreams

## Security, and vulnerability handling 

Foundation staff will collaborate with FreeBSD Project stakeholders (Core, Secteam, Ports Secteam) and downstream vendors (those meeting the CRA definition of *Manufacturers*) to navigate the new regulatory requirements.

The group will develop a shared understanding of responsibilities under the CRA for the Foundation, Project, and vendors. We'll examine potential CRA-related scenarios and determine appropriate collaborative responses.

This collaboration will help all parties assess their evolving responsibilities and needs. The Foundation will lead efforts to scope and cost any new processes or increased workload. We will advocate strongly for additional vendor support to ensure the long-term sustainability of both the Project and Foundation.

This workstream takes a holistic view of FreeBSD's overall security position. We'll update policies, public positions, and documentation as needed to align with CRA requirements.

This workstream will also consider the relevance of emerging good practice from the wider open source ecosystem and adopt these as appropriate.

Duration: 12 months  
Scheduling: Jan 2026 \- Dec 2026  
Resource allocation: 60% FTE   
Target outcomes: 1, 2, 3, and 4 (see “Outcomes” in table above).

## SBOM toolchain 

The Cyber Resilience Act requires [manufacturers](https://digital-strategy.ec.europa.eu/en/policies/cra-summary#ecl-inpage-glossary) to provide an SBOM (Software Bill of Materials) for products covered by the regulation ([REGULATION (EU) 2024/2847](https://eur-lex.europa.eu/eli/reg/2024/2847/oj)).

For FreeBSD and many open source projects, the smartest approach is to create their own SBOM solution. This benefits everyone: downstream manufacturers get an accurate, authoritative SBOM they can rely on, and the FreeBSD Project avoids the headache of dozens of different companies creating their own (possibly inaccurate) SBOMs behind closed doors. By providing a single, shared, open-source SBOM toolchain, it makes life easier for FreeBSD users while maintaining control over how FreeBSD's components are documented.

Development work was started in 2025 under the Infrastructure Modernization project commissioned by the STA, and the Foundation is funding a project extension to continue to mature the SBOM solution.

The project extension will add SBOM information files, identify files with missing licenses and add where possible, update pkgconf for complex licensing schemes, and collaborate with upstream projects to add SBOM metadata where possible.

Duration: 4 months  
Scheduling: Jan 2026 \- April 2026  
Resource allocation: 80% FTE   
Target outcome: 5 (see “Outcomes” in table above).

## Public documentation

The Foundation will collaborate with the FreeBSD Project to publicly document their policy positions regarding the CRA. They will also publish FreeBSD-specific information for [Maintainers](https://digital-strategy.ec.europa.eu/en/policies/cra-summary#ecl-inpage-glossary) and Manufacturers as defined in the CRA. This will cover at least: emerging processes, and contact information. Exact content will be determined as a result of the progress made in the other workstreams.

Duration: 12 months  
Scheduling: Jan 2026 \- December 2026  
Resource allocation: 10% FTE   
Target outcome: 6 (see “Outcomes” in table above).

## Community legislative engagement

The Foundation will establish a simple communication channel (likely a mailing list) to share third-party requests for legislative input with the community.

EU legislative bodies and standardization organizations ([CEN](https://www.cencenelec.eu/about-cen/), [CENELEC](https://www.cencenelec.eu/about-cenelec/), [ETSI](https://www.etsi.org/about)), along with open source collectives, regularly seek input on policy development. Typically, several requests are open at any given time.

While created primarily for CRA-related matters, this channel can also serve for other legislation affecting FreeBSD.

Further thought is needed to determine whether some requests should have a formal or official response, and which are more suited to individual SME input (or both). 

Duration: 12 months  
Scheduling: Jan 2026 \- December 2026  
Resource allocation: 10% FTE  
Target outcome: 7 (see “Outcomes” in table above).

## Public project repo 

A public GH repo (this repo) will be used to document progress on the Foundation’s on CRA Readiness project.

The purpose of this is to provide regular detailed updates about the work done and output produced, as well as showing the decision-making process.

Duration: 12 months  
Scheduling: Jan 2026 \- December 2026  
Resource allocation: 15% FTE   
Target outcome: 8 (see “Outcomes” in table above).

## Communications 

The Foundation will communicate periodically through blogs, social media etc. These communications will aim to share key milestones that have been achieved in the CRA readiness project, share important information, and summarize progress that has been made.

Duration: 12 months  
Scheduling: Jan 2026 \- December 2026  
Resource allocation: 15% FTE   
Target outcome: all outcomes (see “Outcomes” in table above).

# FAQs

>[!Note]
>This FAQ is intended for informational purposes only and does not constitute legal advice. Organizations should consult qualified legal counsel regarding their obligations under the EU Cyber Resilience Act.

### How can I learn more about the CRA?

In these FAQs, the Foundation aims to share the key information you need to know. However, there is far more information about the CRA out there which you can access to learn more. Here are a few resources you may find useful. 

* If you want to see a short intro from the downstream vendors (Manufacturers) side:  
  * [https://www.youtube.com/watch?v=f6V1aregBeU](https://www.youtube.com/watch?v=f6V1aregBeU)   
* If you like reading the original legal text:  
  * Full legal text of CRA [https://eur-lex.europa.eu/eli/reg/2024/2847/oj/eng](https://eur-lex.europa.eu/eli/reg/2024/2847/oj/eng)   
* If you want to see an introduction to CRA at the FreeBSD Vendor Summit by Michael Winser:   
  * [https://youtu.be/MVTCjq0Kg94?si=LCuhlpz8K2mPHd\_F\&t=824](https://youtu.be/MVTCjq0Kg94?si=LCuhlpz8K2mPHd_F&t=824)   
* If you want to see what some of the Open Source Community is doing  
  * Open Regulatory Compliance (ORC) Working Group [https://orcwg.org/](https://orcwg.org/)   
* If you want a CRA 101 from the open source perspective   
  * OpenSSF [https://openssf.org/public-policy/eu-cyber-resilience-act/](https://openssf.org/public-policy/eu-cyber-resilience-act/)   
  * Linux Foundation [https://linuxfoundation.eu/cyber-resilience-act](https://linuxfoundation.eu/cyber-resilience-act)   
* If you want to see the Foundation’s initial statement on the CRA (Feb 2024\)  
  * [https://freebsdfoundation.org/blog/freebsd-foundation-statement-on-the-european-union-cyber-resiliency-act/](https://freebsdfoundation.org/blog/freebsd-foundation-statement-on-the-european-union-cyber-resiliency-act/)   
* If you want to read some CRA FAQs that have been prepared by an open source group  
  * [https://cra.orcwg.org/faq/all/](https://cra.orcwg.org/faq/all/) 

## Overview

### What is the EU Cyber Resilience Act?

The EU Cyber Resilience Act (CRA) is a European Union regulation that establishes cybersecurity requirements for products with digital elements sold or made available on the EU market.

The regulation introduces obligations such as:

* Secure-by-default design  
* Lifecycle vulnerability management  
* Supply chain security and due diligence  
* Security documentation such as Software Bills of Materials (SBOMs)  
* Rapid reporting of actively exploited vulnerabilities

Manufacturers that fail to comply with the regulation may face penalties of up to €15 million or 2.5% of their total worldwide annual turnover, whichever is higher.

### What is a “product with digital elements”?

Under the EU Cyber Resilience Act, a product with digital elements is a software or hardware product that includes software and is placed on the EU market.

Examples may include:

* operating systems and system software  
* network devices and appliances  
* embedded systems  
* connected devices  
* commercial software applications

The regulation primarily targets products placed on the market, not upstream software development projects that publish source code.

### When does the Cyber Resilience Act take effect?

The CRA entered into force on 10 December 2024\.

Key compliance milestones include:

* 11 September 2026 – vulnerability reporting obligations begin  
* 11 December 2027 – the main cybersecurity requirements (including secure-by-default design) apply to products placed on the EU market

Products already on the market before December 2027 are generally only affected if they undergo substantial modification after that date.

## Impact on Open Source

### Does the Cyber Resilience Act apply to open source software projects?

In most cases, open source projects are not the primary targets of the regulation.

The CRA mainly regulates manufacturers placing products on the EU market, rather than collaborative development projects that publish freely available source code.

However, because many commercial products depend on open source components, projects such as the FreeBSD Project may experience indirect effects when downstream vendors work to meet CRA requirements.

### Are individual FreeBSD contributors liable under the CRA?

No.

Individuals contributing to open source projects are generally exempt from obligations under the CRA, even when they are paid to contribute to the project.

Contributing code to the FreeBSD Project does not make a developer responsible for CRA compliance

### What is an “open source steward” under the CRA?

The CRA introduces the concept of an open source steward. This is an organization that supports an open source project but does not place products on the market.

The FreeBSD Foundation is likely to fall into this category, although the exact classification ultimately depends on how the regulation is interpreted and applied in practice.

Open source stewards have limited responsibilities under the CRA and are not subject to the manufacturer penalties defined in the regulation.

Individuals cannot be classified as open source stewards.

### Will the CRA change how open source projects operate?

The CRA does not directly regulate open source development. However, projects that are widely used in commercial products may choose to strengthen practices such as:

* vulnerability disclosure processes  
* security documentation  
* dependency metadata  
* software component inventories

These improvements can help downstream users meet regulatory requirements while maintaining the open development model.

There is active collaboration in the FOSS ecosystem to devise mechanisms to gain more support from manufacturers affected by the CRA.

## Impact on Companies Using FreeBSD

### Who is responsible for CRA compliance when FreeBSD is used in a product?

Responsibility generally lies with the manufacturer or vendor placing the product on the EU market, not with the upstream project.

Companies building products that include components from the FreeBSD Project may need to:

* manage cybersecurity risks across the product lifecycle  
* document software components used in their product  
* provide security updates  
* generate Software Bills of Materials (SBOMs)  
* report actively exploited vulnerabilities

These obligations apply to the product vendor, not to the FreeBSD Project itself.

### Do official FreeBSD releases count as products under the CRA?

The FreeBSD Project publishes source code and binary releases that are freely available for general use.

These releases are typically not considered commercial products placed on the EU market. However, organizations that package FreeBSD into a commercial product or service may have compliance obligations under the CRA.

### What vulnerability reporting deadlines does the CRA require?

If a vulnerability in a product is actively exploited, manufacturers placing that product on the EU market must report it through the CRA reporting system with strict deadlines:

* 24 hours – early warning notification  
* 72 hours – detailed notification  
* 14–28 days – follow-up reporting and remediation updates

These requirements apply to manufacturers of products, not to upstream open source projects themselves.

All such vulnerabilities must be reported on the single vulnerability reporting platform provided by the EU.

## Risks and Challenges for Open Source Projects

### Could the CRA affect the FreeBSD Project indirectly?

Yes.

Even though open source projects are largely exempt from direct regulatory obligations, they may experience operational pressure from downstream manufacturers working to demonstrate compliance.

Examples may include requests for:

* security documentation  
* vulnerability information  
* component metadata  
* SBOM data

### What is a “due diligence denial-of-service” scenario?

Some observers have raised concerns about a potential “due diligence denial-of-service” scenario.

This could occur if a large number of manufacturers simultaneously request documentation or verification information about widely used open source components as part of their CRA compliance processes.

Projects with large downstream user bases may therefore see an increase in compliance-related inquiries.

### Could the CRA affect adoption of FreeBSD?

Potentially.

Manufacturers evaluating software components may increasingly prefer projects that provide:

* clear security processes  
* transparent vulnerability management  
* reliable component metadata  
* SBOM information

Projects that prepare early for these expectations may become more attractive for industry adoption.

## Opportunities for the FreeBSD Ecosystem

### Could the CRA benefit open source projects?

Yes.

The CRA may encourage organizations that rely on open source to invest more in the projects they depend on.

Possible outcomes include:

* funding for upstream development  
* sponsorship of security improvements  
* dedicated maintainers working on upstream projects  
* stronger collaboration between manufacturers and open source communities

Projects that proactively prepare for the new environment may benefit most from these opportunities.

## The FreeBSD Foundation’s CRA Readiness Project

### Why has the FreeBSD Foundation launched a CRA readiness initiative?

The FreeBSD Foundation launched its Cyber Resilience Act Readiness Project in 2026 to prepare the FreeBSD ecosystem for the regulatory changes introduced by the CRA.

The goals of this effort include:

* ensuring the Foundation fulfills its responsibilities as an open source steward  
* protecting the FreeBSD Project from disruption as manufacturers adapt to the CRA  
* helping downstream users understand the information they may need for compliance  
* ensuring that contributors understand they are not personally exposed to liability under the legislation.

### What areas does the CRA readiness project cover?

The initiative includes several workstreams running through 2026\. Please see the top section of this document.

### How is this work being funded?

This work is currently being funded through general donations, which partly come from downstream manufacturers. The Foundation is also seeking specific funding to support the initial readiness phase of the CRA readiness project (through 2026), while aiming to secure targeted ongoing support from the manufacturers who rely heavily on FreeBSD.

### How is the foundation engaging with other FOSS organizations around CRA?

* [https://opensource.org/programs/open-policy-alliance](https://opensource.org/programs/open-policy-alliance)   
* [https://orcwg.org/](https://orcwg.org/)   
* [https://openssf.org/](https://openssf.org/) 

## Practical Questions for Contributors

### Do FreeBSD developers need to change how they contribute?

No major changes are currently required for contributors.

However, improvements to areas such as security documentation, vulnerability handling procedures, and software component metadata may gradually become part of the project’s infrastructure to support downstream users.

### Should contributors worry about legal risk?

No.

The CRA explicitly exempts individual open source contributors from obligations under the regulation.

The FreeBSD Foundation is also working to ensure that the FreeBSD community understands this and that contributors remain protected while the ecosystem adapts to the new regulatory environment.

### Where can contributors learn more about CRA developments affecting FreeBSD?

Relevant resources include:

* Updates from the FreeBSD Foundation  
* Documentation from the FreeBSD Project security team  
* Official materials about the EU Cyber Resilience Act

As the regulatory landscape evolves, these sources will continue providing guidance for the FreeBSD community and downstream users.  
