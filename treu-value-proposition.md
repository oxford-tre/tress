# TREu: a certification-ready University-scale Trusted Research Environment you can share

*A proposition from UCL Advanced Research Computing and the University of Oxford, for expressions of interest and sustainability conversations. October 2026.*

## What TREu is

TREu is the code base behind the UCL ARC Trusted Research Environment. That TRE is live in production at UCL and certified to ISO 27001. Through TRESS (Trusted Research Environments Software Stewardship), a DARE UK–funded project running from September 2025 to January 2027, the University of Oxford has taken the same code and put it to work in a second large institution:

- **TREu** is the original code base, maintained by UCL ARC and running the UCL ARC TRE.
- **TREo** is Oxford’s fork of that code, kept mutually up to date with TREu.
- **TRESS** also refers to the Oxford deployment of TREo, running on AWS and hosting pilot research projects.

Together these show that a production TRE, and the security management that surrounds it, can be shared between sovereign institutions. We are now looking for other institutions and large research projects that want to use TREu or help develop it.

## The problem it addresses

The UK has many University TREs and many TRE code bases. Few are reusable, and fewer still are open source once you count the institutional governance that goes with them. The result is duplicated effort, inconsistent security practice and barriers to collaboration, all of which slow research and raise costs.

Even where TRE code is shared, each organisation must still run its own change control under its own Information Security Management System (ISMS). In practice this means organisations fork open-source TRE code, and the cost of re-approving upstream changes means those forks diverge more or less permanently. TREu takes a different approach: it shares the code, the ISMS, and the processes for changing both.

## What TREu offers

**Certification- and production-ready code and documentation.** UCL ARC runs TREu and its ISMS at scale today. That deployment is certified to ISO 27001 and compliant with the NHS Data Security and Protection Toolkit. An adopter starts from something that has already passed audit, not from a design on paper.

**A Shared Responsibility Model that scales.** TREu is designed to provide a TRE service to a large, varied organisation without the core TRE team becoming responsible for everything. Layered, independent technical controls isolate projects from each other and from IT systems outside the TRE. On top of that isolation, responsibilities are clearly divided:

- project risks are limited by isolation, and residual risks belong to study owners and researchers under well-defined agreements;
- project data remains the responsibility of its information asset owner;
- the compute platform, the TRE team and researchers each have defined duties for keeping the whole system secure.

**Bring your own data and software.** Because projects are strongly isolated, researchers can bring in the software they need rather than choosing from a centrally approved list. Risks from malware or vulnerable software stay inside the project and cannot lead to data leaving the TRE. This suits institutions whose TRE is not itself a data provider and which must support many domains and tool choices.

**Not tied to one cloud.** TREu was designed from the outset to be agnostic to the compute platform. It runs on AWS at UCL and, through TRESS, at Oxford. It is also deployed on UCL's private research computing cloud. Adaptation of TREu to Microsoft Azure and Google Cloud Platform has previously been proposed.

**A reusable ISMS.** UCL’s ISMS is already published openly (isms.arc.ucl.ac.uk) and is being refactored, with a comprehensive implementation guide, so that other institutions can adapt it to their own risk management, access policies and security monitoring, rather than writing their own from scratch.

**An invested community of implementers.** TRESS is developing a documented Software Development Life Cycle (SDLC) that ties code changes to the ISMS. UCL and Oxford call their approach “shared source”: every change is formally controlled at both sites, and where needs differ, the divergence is managed deliberately. The ISMS itself is maintained with the SDLC. TREu is aligned with the SATRE standard architecture and is working towards compliance with K8TRE, so it can use K8TRE-compliant components and contribute its own back to the community.

## What it takes to adopt

TREu is meant to be adopted by a modest team, not built through a large programme.

An adopting organisation would typically need to bring:

| What          | More                                                                                                               | Indicative scale                                                                                       |
|---------------|--------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|
| Engineering   | DevOps time to deploy, operate and co-develop the TRE                                                              | At least 1 FTE recommended                                                                             |
| Cloud account | Cost efficient baseline cloud running costs                                                                        | <£100 per month platform + <£20 per project-month + £5 per user-month + any additional compute/storage |
| Integrations  | Institution identity management, cloud proxying/domains, service management tooling                                | <setup included in engineering>                                                                        |
| Governance    | Technical admins, an ISMS owner and help from Information Governance (IG) to adapt the shared ISMS to local policy | 1 FTE-year to adapt, 2 admins, IG support                                                              |
| Partnership   | Taking part in shared change control with UCL and Oxford                                                           | Regular joint reviews                                                                                  |

## Why a large project or institution might join

**Skip the blank page.** Building and accrediting a TRE from scratch takes years. TREu offers code and an ISMS that are running in production at scale and have already been through ISO 27001 certification.

**Reassure data providers.** A recognised security posture gives data suppliers and controllers confidence in any research domain and reduces the overhead of negotiating data contracts.

**Serve every discipline.** TREu is designed for high volumes of varied projects, spanning medical sciences, the social sciences, the humanities and even libraries. The first pilot at Oxford is studying online arts and culture for young people’s mental health, an NIHR funded collaboration between NHS Trusts, multiple universities, museum and charity partners.

**Steer the roadmap.** Partners co-develop TREu rather than consume it. Planned directions include using local high-performance computing from within the TRE, supporting AI-ready research workflows with software and AI bills of materials, and adopting K8TRE components.

**Join a community, not a vendor.** UCL and Oxford are committed to DARE UK initiatives, to work with partner hospitals and the NHS Thames Valley and Surrey Secure Data Environment, and to publish their outputs openly. Every new partner makes the shared code and practice stronger for everyone.

## Get in touch

We welcome expressions of interest from institutions and large research projects, whether you want to deploy TREu, adapt the ISMS, or collaborate on its development. A first conversation would cover your use cases, preferred cloud platform and governance context.

- **Professor David De Roure**, TRESS lead, University of Oxford: [david.deroure@oerc.ox.ac.uk]
- **Professor Brian Marsden**, University of Oxford Academic Lead for Research Computing and TREs [brian.marsden@cmd.ox.ac.uk]
- **George Svarovsky**, Product Owner, UCL ARC TRE: [g.svarovsky@ucl.ac.uk]
