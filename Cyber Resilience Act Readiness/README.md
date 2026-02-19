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
Resource allocation: 10%   
Target outcome: 7 (see “Outcomes” in table above).

## Public project repo 

A public GH repo (this repo) will be used to document progress on the Foundation’s on CRA Readiness project.

The purpose of this is to provide regular detailed updates about the work done and output produced, as well as showing the decision-making process.

Duration: 12 months  
Scheduling: Jan 2026 \- December 2026  
Resource allocation: 15%   
Target outcome: 8 (see “Outcomes” in table above).

## Communications 

The Foundation will communicate periodically through blogs, social media etc. These communications will aim to share key milestones that have been achieved in the CRA readiness project, share important information, and summarize progress that has been made.

Duration: 12 months  
Scheduling: Jan 2026 \- December 2026  
Resource allocation: 15%   
Target outcome: all outcomes (see “Outcomes” in table above).

# FAQs

We will add FAQs soon. 

Until then, these existing FAQs from the Eclipse Foundation's Open Regulatory Compliance Working Group may be useful. 
  * [https://cra.orcwg.org/faq/all/](https://cra.orcwg.org/faq/all/) 

