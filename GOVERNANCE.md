# CoreDash Project Governance - WIP DRAFT

**Important note**: This governance document is not finalized or implemented at
this time, since we are still in the early days of forming the project. This
document provides people with an opportunity to provide feedback and sets some
initial expectations about the type of governance you can expect coming soon.

The CoreDash umbrella project is composed as a federation of individual projects,
some independent and some interdependent, each of which focuses on some aspect
of CoreDash. Our governance reflects this federated structure.

CoreDash is a Linux Foundation project.

## Individual Subproject Governance

All active Maintainers of each [subproject](subproject.md), are members of that
project's Maintainer Committee, which governs that project.  The subproject's
Maintainer Committee is responsible for the following project governance
activities:

* Ensuring that the subproject creates and publishes regular releases;
* Holding regular, subproject-wide discussions on issues and planning;
* Making final decisions on subproject changes that involve controversial trade-offs;
* Responding to security compromise reports;
* Identifying contributors who are candidates for moving into a maintainer role.

Additionally, each project's Maintainer Committee will select, by majority vote, one
representative to the Steering Committee to be replaced or
renewed by the committee annually.

Should a member of the Maintainer Committee cease being active in the subproject,
violate the Code Of Conduct, or need to be removed for some other reason, they
may be removed by a 2/3 majority vote of the other Committee members, or a
majority vote of the Steering Committee.

## Adopter Council

The Adopter Council exists to represent the needs of CoreDash users. New
members can be added to the Adopter Council by a majority vote of the existing
members.  

The Adopter Council is responsible for the following project governance
activities:

* Review and provide feedback on new projects, roadmaps, and features.
* Hold regular Adopter Council meetings open to all end users and other adopters.
* Gather feedback from CoreDash adopters and share it broadly with the other 
  subprojects and the Steering Committee. 

The Adopter Council will have a chair who is responsible for coordinating
Adopter Council activities. This person will be appointed by the Steering
Committee and will be replaced or renewed by the committee annually.

Should the Adopter Council Chair cease being active in the project,
violate the Code Of Conduct, or need to be removed for some other reason, they
may be removed by a majority vote of the Steering Committee.

## Steering Committee

The overall CoreDash umbrella project is governed by a Steering
Committee, which is selected as follows:

* One Maintainer representative from each member subproject
* One LF representative
* One Adopter Council Chair
* Three Community Representatives

### Steering Committee Duties

The Steering Committee is responsible for the following tasks, any of which may
be delegated to a person or group selected by the committee:

* Reviewing and deciding on new projects to add to CoreDash
* Arbitrating inter-project disagreements
* Ensuring that the LF Code of Conduct is enforced
* Removing projects which have become inactive
* Acting on escalated security or code quality issues
* Resolving issues that individual projects are unable to resolve
* Administering project infrastructure, intellectual property, and resources
* Determining overall direction for advocacy and marketing
* Issuing statements on behalf of CoreDash and its subprojects

In performance of these duties, the Steering Committee will hold a meeting
every other month that is open to all contributors.  The Committee may hold
additional, closed meetings in order to discuss non-public issues such as
security exploits, CoC enforcement, and legal questions.

Steering Committee members are expected to advocate for all of CoreDash, not
just certain projects or corporate sponsors, comply with and support the Code
of Conduct, and be professional and compassionate in all of their dealings with
project participants.

### Steering Committee Elections

In this bootstrapped project phase, the Community Representative(s) will be
appointed. In approximately one year, we will define an election process to
elect future Community Representatives.

## Adding New Subprojects

During the Steering Committee meeting, any project member may recommend
[subprojects](subprojects.md) to become part of CoreDash.  These projects
should have the following characteristics:

* Aligned with the overall CoreDash project;
* Are appropriately licensed and governed or willing to become so;
* Are under active development;
* Consist of high quality code and designs.

The Steering Committee will then review the
application, and decide whether or not to accept it.  If it is accepted, the Committee
will assign one person to assist the subproject in their integration.

## Removing Projects

In some cases, projects will become inactive or unmaintainable, or wish to separate
from CoreDash. Any Steering Committee member may propose removal of a project on
these grounds, and Steering can confirm this with a majority vote.

Projects which still have contributors will then be moved to a repository in their
own namespace.  Projects which have ceased all activity will be archived.


