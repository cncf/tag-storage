# CNCF SIG Storage Graduation Review Project Request

## Harbor Graduation Proposal

Since joining the CNCF in [July 2018](https://www.cncf.io/blog/2018/07/31/cncf-to-host-harbor-in-the-sandbox/) as a Sandbox project and in [November 2018](https://www.cncf.io/blog/2018/11/13/harbor-into-incubator/) moving to an Incubating Project, Harbor has built a healthy ecosystem of users, maintainers, and production implementations.

On behalf of the maintainers team, we believe Harbor is ready for the CNCF [Graduation stage](https://github.com/cncf/toc/blob/master/process/graduation_criteria.adoc#graduation-stage) and meets the v1.2 criteria. We address the CNCF Technical Due Diligence questions in a separate Google Docs document (referred to as the `Tech-DD` from now on).

*Name of project:* Harbor

*Project Description:* Harbor is an open source cloud native registry that provides trust, compliance, performance, and interoperability. As a private on-premises registry, Harbor fills a gap for organizations that prefer not to use a public or cloud-based registry or want a consistent experience across clouds. Harbor secures images with role-based access control, scans images for vulnerabilities, and signs images as trusted. A CNCF Incubating project, Harbor helps you consistently and securely manage images across cloud native compute platforms like Kubernetes and Docker.

Harbor in essense solves common problems in organizations building cloud native applications by offering them a choice to deploy their own private on-premises registry and apply a consistent policy across artifact management in any cloud

Harbor is currently a CNCF Incubating Project. 

## Collateral

**_Link to TOC PR_**

https://github.com/cncf/toc/pull/311

**_Link to Presentation Slides_**

https://docs.google.com/presentation/d/12B5dGc8lMxKeKBFS8pGoldBtZaIWBtDYUFSNcG0mnCc/edit?ts=5d9f4ab2#slide=id.g5d0c4feb44_0_0

**_Link to TOC Presentation_**

https://youtu.be/VRo0U36CZFU?list=PLj6h78yzYM2Mf6GCZzW6CAk6GlZESbemB&t=1785

**_Link to GitHub project_**

https://github.com/goharbor

**_Link to Tech-DD_**

https://docs.google.com/document/d/15gX7EeeXQThEvVMGpL-0a1mOwGuByLtMfvXNJaKT0A0/edit?usp=sharing

**_Link to SIG-Storage Tech-DD for Harbor Graduation_**

http://bit.ly/harbor-graduation-dd

## Summary of Fulfillment of Graduation Requirements
Formal requirements are [here](https://github.com/cncf/toc/blob/master/process/graduation_criteria.adoc).

1. Adheres to TOC Principles and Cloud Native Definition
* [x] Yes
2. Used successfully in production by at least three independent end users which, in the TOC’s judgement, are of adequate quality and scope.
* [x] Yes (many production users are listed in the tech-DD)
3. Have a healthy number of committers, from at least two organizations.
* [x] Yes ([6 organizations have maintainers](https://github.com/goharbor/community/blob/master/MAINTAINERS.md))
4. Demonstrate a substantial ongoing flow of commits and merged contributions.
* [x] [Yes](https://harbor.devstats.cncf.io/d/2/commits-repository-groups?orgId=1&from=now-2y&to=now&var-period=w&var-repogroups=All)
5. Have a clear versioning scheme.
* [x] [Yes](https://github.com/goharbor/harbor/blob/master/RELEASES.md)
6. Have achieved and maintained a Core Infrastructure Initiative Best Practices Badge.
* [x] Yes ([Silver Badge achieved](https://bestpractices.coreinfrastructure.org/en/projects/2095))
7. Have completed an independent and third party security audit with results published of similar scope and quality as provided examples, All critical vulnerabilities need to be addressed before graduation.
* [x] Yes ([Audit by Cure53](https://github.com/goharbor/harbor/blob/master/docs/security/Harbor_Security_Audit_Oct2019.pdf))
8. Explicitly define a project governance and committer process.
* [x] [Yes](https://github.com/goharbor/community/blob/master/GOVERNANCE.md)
9. Have a public list of project adopters for at least the primary repo.
* [x] [Yes](https://github.com/goharbor/harbor/blob/master/ADOPTERS.md)
10. Any other substantive concerns expressed by SIGs or TOC members 
* None

### Summary of what was reviewed, and by who
* Reviewer: Michael Michael (Harbor Maintainer, Director of Product Management at VMware)
* Approver: Saad Ali (CNCF SIG-Storage Tech Lead)

### List of any substantive concerns
* None

### Recommendation to TOC
[x] Graduate
[ ] Not Graduate (Reason(s): )
