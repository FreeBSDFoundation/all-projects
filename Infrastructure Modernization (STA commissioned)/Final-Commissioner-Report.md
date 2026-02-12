### FreeBSD Foundation Final Report to the Sovereign Tech Agency

Jan 30, 2026

### 1\. How Has This Contract Impacted the Open Source Component You Are Working On?

This investment had a meaningful impact on FreeBSD beyond the individual activities funded under the contract. It helped shift both focus and momentum across several critical areas of the Project, particularly around security, sustainability, and community engagement.

Bug management is now more clearly recognized as a shared, community-led responsibility. The work supported under this contract helped elevate bugbusting as a collaborative effort, increasing participation and giving contributors a stronger sense of ownership in improving FreeBSD’s quality and reliability.

The contract also enabled us to set clear technical directions that will shape FreeBSD for years to come. We established a path toward reproducible and zero-trust builds that the community can now adopt and extend. This work reduces security risk, strengthens supply-chain integrity, and increases confidence in FreeBSD build artifacts.

Several efforts initiated through this project are foundational by design. Momentum was established for changes that will take time to fully embed into the Project, including modernization of build processes, vulnerability data handling, and SBOM generation. In each case, the contract allowed us to move from planning to implementation and give the community a concrete starting point for continued progress.

### 1b. What Would You Like to Share with the Public About the Progress You Made During the Contracted Period?

The goal of this project was to modernize key elements of FreeBSD’s infrastructure in ways that improve both security management and developer experience. During the contract period, we made substantial progress toward those goals.

On the security side, FreeBSD can now import, store, and export vulnerability data using the industry-recognized OSV format. This makes our data compatible with widely used third-party tools and reduces friction for downstream users and organizations that rely on FreeBSD. The tooling developed through this work is available for the community to adopt and integrate into its processes.

We also made progress on generating Software Bills of Materials for third-party components included in FreeBSD. While this solution is not yet comprehensive, it establishes a critical foundation for regulatory compliance, including the EU Cyber Resilience Act. The FreeBSD Foundation continues to fund and advance this work into 2026\.

In addition, FreeBSD can now be built reproducibly and without root privileges. This reduces attack surface, enables verification of build artifacts against source inputs, and increases confidence for users deploying FreeBSD in sensitive environments.

From a developer experience perspective, upcoming CI/CD improvements will allow contributors to test changes earlier and on their own hardware. Community-led bug management has also increased, supported by improvements to Bugzilla and better bug backlog analysis tooling, empowering developers to identify and fix issues more effectively.

### 2\. What Impact Did the Financial Support Have on Your Team, Your Organization, and the Community?

The scale and structure of this investment had a significant positive impact on the Foundation and the FreeBSD community. It gave us the ability to plan, coordinate, and manage a project of this size with intention rather than in a purely reactive mode.

The Foundation was able to bring new developers into the project and deepen engagement with upstream initiatives such as OSV, PURL, and pkgconf. These collaborations strengthened technical alignment across projects and exposed the FreeBSD community to different approaches and best practices.

Recognition from a respected organization like the Sovereign Tech Agency reinforced the importance and relevance of FreeBSD as a critical digital infrastructure. That validation had a meaningful impact not only within the FreeBSD community, but also across the broader technology ecosystem that depends on FreeBSD.

### 3\. What Challenges Did You Face While Working on This Project?

This project faced several challenges related to timing, capacity, and external dependencies.

The contract was signed later than expected, but the project timeline was not adjusted to reflect this. As a result, the team experienced time pressure early in the project and needed to catch up while work was already underway.

Planning for some work packages coincided with a seasonal slowdown and a limited pool of qualified contractors. At the same time, the FreeBSD Foundation was planning another large initiative, the Laptop Support and Usability Project, which drew on the same management resources. Balancing multiple time-sensitive efforts required careful prioritization.

Contractor availability was a recurring constraint. The work required highly specialized expertise, and many contractors were also FreeBSD volunteers with competing demands on their time. Estimating hours proved difficult due to variable contract structures, and the Foundation’s small staff meant that covering holidays or absences added additional pressure.

Finally, progress depended in part on volunteer review cycles, release schedules, and security team processes that we could not fully control. Some work packages were also not entirely “shovel-ready,” as fully scoping them in advance would have required significant volunteer time without certainty of funding.

Despite these challenges, the project delivered meaningful outcomes and set durable technical directions for the future.

### 4\. What’s Next for the Open Source Component, Your Team, or Your Organization?

Several efforts initiated under this contract are continuing. Ongoing work on SBOM generation remains a priority, as does completing and integrating CI improvements currently underway.

Looking ahead, we are focused on improving contributor experience through modernization of project tooling, including Forgejo infrastructure. We are also shaping a long-term security posture informed by regulatory realities such as the EU Cyber Resilience Act, with an emphasis on sovereignty, resilience, and sustainability.

To support this vision, the Foundation is exploring ways to secure ongoing funding for critical roles such as system administrators and a dedicated security officer, positions that are essential to maintaining FreeBSD as reliable, long-term infrastructure.