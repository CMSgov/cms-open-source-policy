# Introduction

The [Centers for Medicare & Medicaid Services (CMS)](https://www.cms.gov) has been an active supporter of and has utilized the [Open Source Software (OSS)](https://www.cms.gov/tra/Application_Development/AD_0200_Open_Source_Introduction.htm) on several IT projects for its mission-critical programs. Several CMS business units and offices have been actively releasing OSS as part of IT modernization projects. CMS has many active open source communities, such as our [Developer APIs](https://developer.cms.gov/#apis) like [Bluebutton](https://bluebutton.cms.gov/), our [CMS Design System](https://developer.cms.gov/design-system/), and hundreds of other repos across [our many organizations](https://dsacms.github.io/metrics/organizations/). CMS has embraced Open Source development and is looking forward to releasing software to the community to promote reuse. This policy will help CMS achieve the goals outlined in the [OMB directive M-16-21](https://www.whitehouse.gov/wp-content/uploads/legacy_drupal_files/omb/memoranda/2016/m_16_21.pdf) for Federal agencies.

## OSS Consideration & Applicability

This policy applies to the CMS project teams that engage in the development of code for the Open Source community. This policy assumes that before OSS development, and in accordance with the [three-step software solution analysis](https://code.gov/agency-compliance/compliance/procurement), the project team has conducted market research and analyzed commercial and other open source alternatives that may meet their business need. This OSS policy applies when the project team ventures into custom code development and chooses the project code as a candidate for OSS.

The project teams must verify [if they may not release](https://www.whitehouse.gov/wp-content/uploads/legacy_drupal_files/omb/memoranda/2016/m_16_21.pdf) the source code that has been developed using Government funds. Applicable exceptions are as follows:

> 1. The sharing of the source code is restricted by law or regulation, including—but not limited to—patent or intellectual property law, the Export Asset Regulations, the International Traffic in Arms Regulation, and the Federal laws and regulations governing classified information;
> 2. The sharing of the source code would create an identifiable risk to the detriment of national security, confidentiality of Government information, or individual privacy;
> 3. The sharing of the source code would create an identifiable risk to the stability, security, or integrity of the agency’s systems or personnel;
> 4. The sharing of the source code would create an identifiable risk to agency mission, programs, or operations; or
> 5. The CIO believes it is in the national interest to exempt sharing the source code. For excepted software, agencies must provide OMB a brief narrative justification for each exception, with redactions as appropriate.

## Government Data Rights

The CMS Office of Acquisition and Grants Management (OAGM) has an established IT procurement procedure that sets the [rights to the custom-developed code](https://www.acquisition.gov/far/subpart-27.4) including at a minimum, rights to Government-wide reuse and rights to modify the code. CMS contractors who develop software for CMS business use are covered by the procurement clauses that provide the Copyright of the CMS-funded custom designed software to CMS and prohibits the contractors from reselling it to other Federal Government agencies. Such custom produced software for CMS can be made freely available to other Government agencies. Due to a variety of IT and non-IT contracts that CMS may enter into, it is the project team’s responsibility to perform all due diligence for their specific contract in consultation with the OAGM. CMS requires all development contractors to maintain the source code and documentation in a CMS-approved and accessible version control system. CMS has created the [target lifecycle governance framework](https://www.cms.gov/data-research/cms-information-technology/tlc) for the development teams to identify, track and maintain version control of all software artifacts. The [TLC artifacts are deliverables](https://www.cms.gov/files/document/cms-tlc-guidance-document-2023.pdf) to CMS that provide a set of documentation and source code that might be considered for Government-wide reuse of the custom software.

## CMS OSS Pilot Program

As outlined in the requirements of the [Federal Source Code Policy](https://code.gov/#/policy-guide/policy/introduction), CMS has already identified the [Quality Payment Program (QPP)](https://qpp.cms.gov/) as CMS’ OSS pilot program. The QPP project team has already released [a tool for file conversion](https://github.com/CMSgov/qpp-conversion-tool) as OSS during the calendar year 2017. The QPP conversion tool allows XML to JSON file conversion for consumption by the Submissions API. The project team believes that it will let any provider or entity that creates QPP files have access to the tool outside of the context of QPP submissions and that can be extended to other file formats.

CMS intends to release additional OSS as the QPP program matures.

## OSS Implementation & Infrastructure

Any CMS project team that wishes to publish their code as OSS must set a clear expectation of their level of involvement in sustaining that project. The project team shall define an OSS release process that begins with a determination of if the intended software can indeed be released as OSS, considering any security and other CMS policy restrictions. Depending on the nature of the OSS and associated licensing model, the project team shall adequately allocate resources to be able to sustain and flourish the project in the open source community.

The project team shall utilize an existing public-facing website to convey information about the project and provide a link to the project’s GitHub repository. The project team should implement tools to support the community around an open source project, such as mailing lists, message forums, a version control, wiki, and tracking mechanisms, such as Kanban boards to track issues and bugs on the GitHub repository.

For every iteration of the code release, the project team must ensure that the software code is adequately peer reviewed for security vulnerabilities that can be exploited by malicious actors and that any discovered vulnerabilities are removed prior to release. Until the software code is adequately reviewed, it should be either 1) maintained in an internal code repository that replicates the intended public repository or 2) checked by publicly available services providing the same functions on all code check-ins to the public source code repository. The software should also contain automated unit tests and build scripts and should be [checked for software vulnerabilities](https://github.com/DSACMS/repo-scaffolder/tree/main/tier3/checklist.md#code-analysis), [code quality](https://github.com/DSACMS/repo-scaffolder/tree/main/tier3/checklist.md#code-review) and code coverage [using available standard CMS tools and guidance](https://github.com/DSACMS/repo-scaffolder). The code should be released using [open source best practices and standards](https://github.com/DSACMS/repo-scaffolder/blob/main/tier3/%7B%7Bcookiecutter.project_slug%7D%7D/MAINTAINERS.md#tier-3-release-guidelines), and when possible built and verified via an automated continuous integration/continuous deployment process. The project team should [include ample documentation](https://github.com/DSACMS/repo-scaffolder/tree/main/tier3) with the software code for increased adoption and modification by the community. The documentation should provide the information on [project’s mission, philosophy, goal, design](https://github.com/DSACMS/repo-scaffolder/blob/main/tier3/%7B%7Bcookiecutter.project_slug%7D%7D/README.md#about-the-project), [decision-making process](https://github.com/DSACMS/repo-scaffolder/blob/main/tier3/%7B%7Bcookiecutter.project_slug%7D%7D/GOVERNANCE.md), product roadmap and [instructions on how to submit issues, feature requests and how to contribute towards a fix or enhancements](https://github.com/DSACMS/repo-scaffolder/blob/main/tier3/%7B%7Bcookiecutter.project_slug%7D%7D/CONTRIBUTING.md). The documentation should be accessible to the Open Source community via the repository.

CMS project teams should follow or adopt a decentralized governance model to ensure the success of the OSS as the software matures in the Open Source community. The governance model should define the team constituents, their decision-making authority and their [roles](https://github.com/DSACMS/repo-scaffolder/blob/main/tier3/%7B%7Bcookiecutter.project_slug%7D%7D/MAINTAINERS.md) to support the project in the open source community. For sustaining the project, the team, at a minimum, should define and staff the roles for active user engagement, product roadmap development, and accepting new contributions via pull-requests. These resources shall be staffed in addition to existing project team members. The project team is expected to take on the additional responsibility of encouraging meaningful engagement in the project by identifying and promoting active contributors to committer status based on the quality and quantity of code contributions and involvement in day-to-day discussions.

## CMS' Public OSS Repositories

CMS project teams shall utilize official Public CMS GitHub organization accounts to make their source code available to the open source community and for government-wide use. The project teams shall use a consistent naming convention and a prefix for their code repository names (e.g. bluebutton-web-server) and utilize [repository topics](https://github.com/DSACMS/repo-scaffolder/blob/main/tier3/checklist.md#review-repository-details) to improve identification on GitHub. The project teams shall also provide updates to the [CMS’s official enterprise code inventory](https://dsacms.github.io/metrics/projects/), update the [repository's code.json](https://github.com/DSACMS/repo-scaffolder/blob/main/README.md#add-codejson-to-your-project) and, update the CMS enterprise code repository at Code.gov to encourage discovery and dissemination of the software.

## License

For CMS projects using OSS, each CMS business owner is responsible for assuring that CMS’s use of the open source is according to license. For a CMS-released OSS project, the CMS business owner is responsible for selecting an appropriate license model. In either case, the TRB is responsible for approval of OSS licenses.
Be aware of licensing issues and select a licensing model considering the difference between “permissive” and “non-permissive” licenses, warranty / guarantee limitations, attribution, and trademark / IP protections and its impact on the choice of license.

Our default LICENSE file for projects acknowledges that our work is in the U.S. public domain, and uses [Creative Commons Zero International 1.0 (CC0)](https://creativecommons.org/publicdomain/zero/1.0/) to waive copyright internationally. The [Open Source Initiative maintains a list of licenses](https://opensource.org/licenses?categories=popular-strong-community) that the project team may optionally use. In addition to obtaining TRB approval, the Office of General Counsel must review any proposed open source modification or creation.

A useful resource is Open Source Licenses is [tl;dr legal's verified license resource page](https://www.tldrlegal.com/verified#verified-licenses).

The CMS Technical Reference Architecture (TRA) Volume IV [“Development and Application Services”](https://www.cms.gov/tra/Application_Development/AD_0010_Application_Introduction.htm) provides additional guidelines for the CMS project team that wish to use the OSS libraries and packaged OSS for their internal consumption or development of new and custom software that is not intended for the publication in the OSS community.

## Transition and End of Life (EOL) considerations

A CMS OSS project may be retired due to inactivity, or due to a compelling business need, or transition of project to other organizations. When ending support, projects should send a notification to existing end users, informing them of CMS’s decision to terminate support of the OSS.

## Acknowledgments

The utilization, development, and adoption of OSS at CMS would not be possible with the guidance and support of [The Digital Service at the Centers for Medicare & Medicaid Services](https://cms.gov/digital-service), [The Department of Health and Human Services](https://hhs.gov), and [The United States Digital Service](https://www.usds.gov).

CMS would like to thank the following agencies for their inspirational work in the use of Free/Open Source Software in the Federal Government:

- [18F](https://github.com/18F/open-source-policy/blob/master/policy.md)
- [Consumer Financial Protection Bureau (CFPB)](https://github.com/cfpb/source-code-policy/blob/gh-pages/cfpb-source-code-policy.md)
- [Cybersecurity and Infrastructure Security Agency (CISA)](https://github.com/cisagov/development-guide/blob/develop/open-source-policy/policy.md)
- [Department of Homeland Security (DHS)](https://www.dhs.gov/scip)
- [General Services Administration (GSA)](https://open.gsa.gov/oss/)
- [Office of Management and Budget (OMB)](https://www.whitehouse.gov/wp-content/uploads/legacy_drupal_files/omb/memoranda/2016/m_16_21.pdf)

Our work continues to be guided by contributions from:

- [CHAOSS OSPO Metrics Working Group](https://chaoss.community)
- [TODOGroup](https://todogroup.org)
- [US Digital Response](https://www.usdigitalresponse.org)

Finally, thank you to all the open source contributors sending PRs, filing issues, and advocating for this important work across the ecosystem!

## Future changes

This CMS policy is a living document, and any changes to this policy in the future would be handled via issues and pull requests in the [CMS GitHub repository](https://github.com/CMSgov/cms-open-source-policy).
