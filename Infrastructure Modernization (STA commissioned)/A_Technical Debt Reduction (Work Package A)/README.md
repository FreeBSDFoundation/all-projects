#  The FreeBSD Foundation's *STA Work Package A - Tech Debt Project*

| Project Name | STA Work Package A - Pay down technical debt and implement tools and processes to keep it low|
| :---- | :---- |
| Comissioning Body | Sovereign Tech Agency |
| Funding Status | Approved on August 26, 2024 |
| Project Sponsor | [Ed Maste](https://github.com/emaste) |
| Project Manager | [Alice Sowerby](https://github.com/alice-sowerby) |
| Objectives | Perform bug triage and remediation, document patches and fixes, develop a comprehensive issue management program, and assess and implement issue management tools and technologies. |
| Organization goals |The number of open bugs in the FreeBSD base system, exceeding 7,000, is unsustainable. Many of these are old and are likely obsolete either because they refer to earlier versions, or they have been overcome by other development work. <br/><br/>Some are higher priority than others and must be reviewed and addressed with some urgency. <br/><br/>The number of bugs and the average open duration is not healthy for the project. For FreeBSD users, both current and potential, such a high number of bugs reduces confidence in the quality of the code. For developers and users who submit bugs, a slow review and remediation process reduces engagement, something the project can’t afford given the need to grow the developer community.  <br/><br/>The goal of this work package is to reduce the number of open bugs to the 10-year historical average of x. This work package will also develop a comprehensive vulnerability management process that, in combination with the implementation of new tooling, will keep the number of open bugs and average open duration within acceptable ranges. |
| Output | Reduction in open bugs to the 10-year historical average. New processes and tooling to facilitate long term control over the growth of open bugs |

## Stakeholder Analysis

R = Responsible, A = Accountable , C = Consulted, I = Informed

* Core and SrcMgr teams - A, C, I
* Assigned developer(s) - R, C, I
* Alice Sowerby (Project Manager) - R, C, I
* Ed Maste (Technical Sponsor) - R, A, C, I
* Deb Goodkin (Executive Sponsor) - A, I
* Sovereign Tech Agency (Commissioning Body) - A, I

## Scope
| Within Scope| Outside Scope           |
|:------------|:--------------------------|
| Reduce open bugs to historical 10-year average | One reason, perhaps a main reason, why there are so many open bugs is because there are too few committers to review and merge. <br/><br/>Addressing the Committer shortfall is out of scope.  |
| Assess vulnerability management tools and processes, recommend and implement improvements| | 
| Write documentation to accompany new processes and tools | | 

## Quick links
[Latest Updates](https://github.com/FreeBSDFoundation/Project-STA-A-Tech-Debt/tree/main/Updates)

[Meeting Notes](https://github.com/FreeBSDFoundation/Project-STA-A-Tech-Debt/tree/main/Meeting-Notes)

[Foundation blog about the Sovereign Tech Agency commission](https://freebsdfoundation.org/blog/sovereign-tech-fund-to-invest-e686400-in-freebsd-infrastructure-modernization/)

To learn more about FreeBSD bug triage and remediation in general, please refer the following links:
[https://www.freebsd.org/administration/#t-bugmeister](https://www.freebsd.org/administration/#t-bugmeister)

[https://bugs.freebsd.org/bugzilla/](https://bugs.freebsd.org/bugzilla/)

## Discussion threads
We support the FreeBSD mailing lists as the community's preferred way to discuss all FreeBSD matters.

[FreeBSD Bugs Mailing List](https://lists.freebsd.org/subscription/freebsd-bugs)

[All FreeBSD Mailing Lists](https://lists.freebsd.org/)

## FAQs

### How much is being invested in this work?

The total value of the STA commission is €686,400 to drive improvements in infrastructure, security, regulatory compliance, and developer experience.

### How long is this program due to run?

The program will start in August 2024 and end in December 2025.

### How was the scope of the work decided? 

The high-level scope was outlined by the FreeBSD Foundation with input from the community, including key stakeholders identified earlier in this document.

### What exactly is covered in the planned work?   
The scope will be unpacked month by month as we make progress, focusing on where the most high-value functionality can be achieved with the resources and support that we have available. Check out the [Meeting Notes](https://github.com/FreeBSDFoundation/Project-STA-A-Tech-Debt/tree/main/Meeting-Notes) to see how the work is being discussed over time.

### Who will be doing the work?

The Foundation will be managing staff and a group of contracted FreeBSD developers to work on different functional areas to deliver regular updates on the project goals. 

### How can I share my views on what would make this project better?
If your suggestions are suitable for public discussion, we ask that you start a conversation in the most suitable [FreeBSD mailing list](https://lists.freebsd.org/) or you can reach the Foundation through the usual channels [https://freebsdfoundation.org/about-us/contact-us/](https://freebsdfoundation.org/about-us/contact-us/).

### How can I keep up to date with the work in progress and any new releases?

There are several ways to keep yourself in the loop. 

1. Read the [monthly updates](monthly-updates) that are posted into this repo.
2. Seek out the recordings of the Technology Team Updates given at BSD conferences such as BSDCan.
4. Read the quarterly reports on FreeBSD.org
5. Sign up to the FreeBSD Foundation newsletter. All announcements about the program will be included in our updates.

### How is this repo being used by the Foundation for this project?
We are using this repo to capture key project information and updates. We are not using it for source code management. The repo is read-only for the public.