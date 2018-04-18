Introduction

The [Centers for Medicare and Medicaid Services (CMS)](https://www.cms.gov) has been an active supporter of and has utilized the [Open Source Software (OSS)](https://en.wikipedia.org/wiki/Free_and_open-source_software) on several IT projects for its mission-critical programs. Several CMS business units and offices have been actively releasing OSS as part of IT modernization projects. CMS has many active open source communities, such as the BlueButton, [Healthcare.gov](http://healthcare.gov/) StyleGuide, and the MMIS Provider screening module on Github. CMS has embraced the OSS for our development projects and is looking forward to releasing software codes to the open source community to promote its reuse. This policy will help CMS achieve the goals outlined in the [OMB directive](https://code.gov/#/policy-guide/policy/introduction) for Federal agencies.

OSS Consideration & Applicability

This policy assumes that before OSS development, and in accordance with the three-step software solution analysis, the project team has conducted market research and analyzed commercial and other open source alternatives that may meet their business need. This OSS policy applies when the project team ventures into custom code development and chooses the project code as a candidate for OSS.  The project teams must verify if they may release the source code that has been developed using Government funds.

Government Data Rights

The CMS Office of the Acquisition and Grants Management (OAGM) has an established IT procurement procedure that sets the rights to the custom-developed code, including at a minimum, rights to Government-wide reuse and rights to modify the code.  CMS contractors who develop software for CMS business use are covered by the procurement clauses that provide the Copyright of the CMS-funded custom designed software to CMS and prohibits the contractors from reselling it to other Federal Government agencies. Such custom produced software for CMS can be made freely available to other Government agencies. Due to a variety of IT and non-IT contracts that CMS may enter into, it is the project team’s responsibility to perform all due diligence for their specific contract in consultation with the OAGM. The project team shall review Section 21: “Logistic Considerations”, and section 5.27: “Contractor Data Requirements” of OAGM Acquisition Plan Guide before releasing the code as OSS. CMS requires all development contractors to maintain the source code and documentation in a CMS-approved and accessible version control system. CMS has created eXpedited LifeCycle (XLC) process framework for the development teams to identify, track and version control all software artifacts. The XLC artifacts are deliverables to CMS that provides a set of documentation and source code that might be considered for Government-wide reuse of the custom software.

 

CMS OSS Pilot Program

As outlined in the requirements of the Federal Source Code Policy, CMS has already identified the Quality Payment Program (QPP) as CMS’ OSS pilot program. The QPP project team has already released a tool for file conversion as OSS during the calendar year 2017. The QPP conversion tool allows XML to JSON file conversion for consumption by the Submissions API.  The project team believes that it will let any provider or entity that creates QPP files to have access to the tool outside of the context of QPP submissions and that can be extended to other file formats.

CMS intends to release the additional OSS as the QPP program matures.

OSS Implementation & Infrastructure

Any CMS project team that wishes to publish their code as OSS must set a clear expectation of their level of involvement in sustaining that project. The project team shall define an OSS release process that begins with a determination of if the intended software can indeed be released as OSS, considering any security and other CMS policy restrictions. Depending on the nature of the OSS and associated licensing model, the project team shall adequately allocate resources to be able to sustain and flourish the project in the open source community.

The project team shall utilize an existing public-facing website to convey information about the project and provide a link to the project’s GitHub repository. The project team should implement tools to support the community around an open source project, such as mailing lists, message forums, a version control, wiki, and tracking mechanisms, such as Kanban boards to track issues and bugs on the GitHub repository.

For every iteration of the code release, the project team must ensure that the software code is adequately peer reviewed and is free of security vulnerabilities that can be exploited by malicious actors. Until the software code is adequately reviewed, it should be either 1) maintained in an internal code repository that replicates the intended public repository or 2) checked by publicly available services providing the same functions on all code check-ins to the public source code repository. The software should also contain automated unit tests, build scripts and should be checked for software vulnerabilities, code quality and code coverage using available standard CMS tools. The code should be built with CMS’s standard continuous integration (CI) server. The project team should include ample documentation with the software code for increased adoption and modification by the community. The documentation should provide the information on project’s mission, philosophy, goal, design, decision-making process, product roadmap and instructions on how to submit issues, feature requests and how to contribute towards a fix or enhancements. The documentation should be accessible to the Open Source community.

The CMS project teams should follow or adopt a decentralized governance model to ensure the success of the OSS as the software matures in the Open Source community. The governance model should define the team constituents, their decision-making authority and their roles to support the project in the open source community. For sustaining the project, the team, at a minimum, should define and staff the roles for active user engagement, product roadmap development, and accepting new contributions via pull-requests. These resources shall be staffed in addition to existing project team members. The project team is expected to take on the additional responsibility of encouraging meaningful engagement in the project by identifying and promoting active contributors to committer status based on the quality and quantity of code contributions and involvement in day-to-day discussions, as is the case in a meritocracy based system.

 

CMS' Public OSS Repository

The CMS project teams shall utilize the official CMS GitHub organization account to make their source code available to the open source community and for Government-Wide use. The project teams shall use a consistent naming convention and a prefix for their code repositories that allows for easy identification on GitHub. The project teams shall also provide updates to the CMS’s official enterprise code inventory, update the CMS public website - the OSS landing page and, update the CMS enterprise code repository at Code.gov to encourage discovery and dissemination of the software. 

License

There is a wide variety of OSS licensing models available, and the CMS project teams are required to research and choose a licensing model that is suitable for their project. Several CMS projects have preferred to dedicate their work in the Public Domain.  The Open Source Initiative maintains a list of licenses that the project team may optionally use. The section Choosing a License at the Civic Commons wiki may also be a useful resource that provides additional help for selection of an appropriate license. The project team should consider the difference between “permissive” and “non-permissive” licenses, warranty/guarantee limitations, attribution, and trademark/IP protections and its impact on the choice of license.

Once an appropriate license is chosen for the project, the full license text should be included in the ‘license’ file of the distribution bundle. Each source code must have a notice at the top to name CMS, or an organization designated explicitly by CMS as the copyright and license holder of the source code and provide a link to the full text of the license.

The project team must perform appropriate due diligence before the publication of their source code, primarily when the project team uses or imports any freely available open source products and libraries to build their software that is released as OSS. The original license of all referenced code and libraries must be included with the distribution of the source, according to the terms of the original license. The CMS Technical Reference Architecture (TRA) supplement “Development and Application Services” provides additional guidelines for the CMS project team that wish to use the OSS libraries and packaged OSS for their internal consumption or development of new and custom software that is not intended for the publication in the OSS community.

Transition and End of Life (EOL) considerations

A CMS OSS project may be retired due to inactivity, or due to a compelling business need, or the project transitioned to other organizations. When ending support, projects should send a notification to existing end users, informing them of CMS’s decision to terminate support of the OSS.

Acknowledgments

CMS would like to thank General Services Administration (GSA)’s 18F team, the Consumer Financial Protection Bureau (CFPB), and the Office of Management and Budget (OMB) for their inspirational work in the use of OSS in the Federal Government.

Future changes

This CMS policy is a living document, and any changes to this policy in the future would be handled via issues and pull requests in the CMS GitHub repository.

