[[ccs-reference]]
== Overview

This is the documentation of CCS version 1.0.0.

[float]
=== What is CCS?

The Customs Common Schema (CCS) is an proprietary specification that defines a common set of fields to be used when storing customs data in JSON, such as declarations and notifications.

CCS specifies field names and eCustoms.cloud datatypes for each field, and provides descriptions and example usage. CCS also groups fields into CCS levels, which are used to signal how much a field is expected to be present. Finally, CCS also provides a set of naming guidelines for adding custom fields.

The goal of CCS is to enable and encourage eCustoms.cloud users to normalise their customs, transport and trade data, so that they can better analyse, visualise, and correlate the data represented in their transactions. CCS has been scoped to accommodate a wide variety of events, spanning:


- *Event sources*: whether the source of your event is an Elastic product,
  a third- party product, or a custom application built by your organization.
- *Ingestion architectures*: whether the ingestion path for your events includes Beats processors,
  Logstash, Elasticsearch ingest node, all of the above, or none of the above.
- *Consumers*: whether consumed by API, Kibana queries, dashboards, apps, or other means.

[float]
=== New to CCS?

If you're new to CCS and looking for an introduction to its benefits and examples of the
core concepts, <<ccs-getting-started>> is a great place to start.

[float]
=== My events don't map with CCS

CCS is a permissive schema. If your events have additional data that cannot be
mapped to CCS, you can simply add them to your events, using custom field names.


[float]
=== Maturity

CCS improvements are released following https://semver.org/[Semantic Versioning].
Major CCS releases are planned to be aligned with major Elastic Stack releases.

Any feedback on the general structure, missing fields, or existing fields is appreciated.
For contributions please read the
https://github.com/elastic/ecs/blob/master/CONTRIBUTING.md[Contribution
Guidelines].



include::using.asciidoc[]
include::fields.asciidoc[]
include::field-values.asciidoc[]
include::migrating.asciidoc[]
include::additional.asciidoc[]
