# Welcome to the CoreDash Community!

With the recent license changes of the Grafana project, there are quite a few
community end users as well as monitoring vendors who are interested in a
PromQL visualization and dashboarding solution that is under the Apache-2.0 
license, owned by the Linux Foundation, and governed by a mix of community
end users and vendors. The CoreDash Project is designed as a place where we can
work together on this solution. Please note that CoreDash is not designed to be
a fork of Grafana, but will instead take a more componetized approach as a
collection of subprojects that users can select from to meet their needs.

CoreDash is the current working name / code name for this effort, but we expect
to rename it after we've made a bit more progress and better defined what we
plan to do.

## Getting Started

### Communication

Please join the coredash-discuss@googlegroups.com 
[mailing list](https://groups.google.com/g/coredash-discuss)
where we have discussions about the project.

We meet on the 1st and 3rd Thursday of every month at 7am PT | 10am ET | 15:00 UK
for 1 hour. Agendas, meeting notes, and joining details can be found in our
[working session
doc](https://docs.google.com/document/d/1FZy-tuIz-C5NSQe3AdeT-DixZZXMjDi-BnQy2kj_9xU/edit).
 
Participation in this community is subject to our
[Code of Conduct](CODE_OF_CONDUCT.md).

### Subprojects

You can start now by contributing to one of our [subprojects](subprojects.md). 

If you have a project (or want to start one) that would be a good fit for this
effort, please reach out on the mailing list to discuss contributing a new
subproject to this Linux Foundation effort.

## Scope

If we look at the Observability and Analysis segment of the CNCF Landscape, the
three projects in metrics based monitoring (Prometheus, Cortex and Thanos) are
all Prometheus ingest format and PromQL based solutions. The other graduated or
incubating projects are fluentd in logging which has no standard ingest protocol
or query language yet and Jaeger and OpenTracing, which have a standard
protocol, but customized visualization / UX per solution.

To give this new project the best chance of being successful, reducing the initial
scope to provide faster value for end users is ideal from our perspective.
Therefore, having a visualization project that is focused on Prometheus and
PromQL seems to be a logical starting point. Most open source and vendored
solutions in the CNCF Monitoring landscape support both Prometheus ingestion
format as well as PromQL. 

Perhaps over time, the project can look to add other industry standard
monitoring protocol support like Graphite or expand into visualization for
logging and distributed traces, but to start, the focus will be on deriving
value for one use case (Prometheus/PromQL) and building up from there versus
attempting to replicate all of the various visualization capabilities of
Grafana.

The project will also improve the state of the art for finding and choosing
Prometheus metrics to visualize, and for constructing PromQL queries.

## Draft Goals

Goals are broken down into two sections: 1) Dashboards and 2) Ease of querying. 

**Dashboards**:
Core visualization goals which are focused on visualization of metric data
based on PromQL and allowing users to create savable and shareable dashboards
from them:

* Visualization:
  * Visualization of multiple metric time series data in a single chart from one
    or more queries.
  * Ability to compose multiple charts together into a dashboard.
  * Ability to store, retrieve, update, delete and share dashboards.
  * Ability to parameterize charts.
  * Ability to adjust the lookback window.
  * Ability to choose settings once for a dashboard and have those settings apply
    to multiple charts in the dashboard. 
  * Configurable ability to gracefully degrade the visualization behavior when
    query result sets are very large.
* Configuration & Management:
  * Explicit externalized data model.
  * Ability to manage lifecycle and configuration of dashboard definitions using a
    GitOps model.
  * Ability to migrate from other/legacy dashboard formats, specifically including
    Grafana dashboard definitions.
* Extensibility & Reuse:
  * Deliver as both a library and an application.
  * Charts and dashboards can easily be placed inside other applications and other
    use cases.
  * Future: Ability to extend visualizations to other chart types.
  * Future: Ability to extend query language to others.
  * Future: Ability to extend visualization to other data types like logs and
    distributed traces.
 
**Ease of Querying**:
Goal focused on helping beginners and first time users of PromQL to craft their
queries. If PromQL is going to be the long term industry standard open source
query language, many more end users will have to become familiar with it over
time:

* Visual Query builder to help users construct PromQL queries.
* Query Analyzer to help users identify inefficiencies in their queries.
* Prompts and libraries/catalog of common or example queries to help users get
  started.

The target user would be a JavaScript developer.

## License

This project is Licensed under [Apache 2.0](LICENSE).
