---
layout: default
title: "SCS - Self-Contained Systems - Why?"
---

Why SCS?
---

There are many reasons why we think SCS are appealing. This page gives
and overview of the most important ones.

### Disappointed by Monolith

Monoliths are large applications that can be deployed as a whole. They
are hard to develop and maintain in the long run. The architecture
rots because it is to easy to introduce new dependencies - all it
takes is a developer who decides to use a class in a piece of code
where he/she really shouldn't. Also it takes long and it is complex to
test and deploy the monoliths. Finally if the monolith cannot be
maintained any more it is essentially impossible to replace it. So we
need smaller deployment units that still fit a business purpose and
ideally also influence the organization.

### Local Decisions

A decision for a technology or architecture in one SCS is local to
that SCS. Changes for new requirements should be limited to one SCS as
it implements a functionality all by itself. Pretty much all decisions
concerning technology and a lot concerning architecture are local to a
single SCS. We have seen a lot of large monoliths fail. More
isolations on the architectural level promises to make even large
projects feasible.

### Isolation

An SCS is a natural unit in many regards. If one SCS fails it will not
influence the other SCS just because it is a separate process and does
not really interact with the other SCS. This makes high-availability
easier. Also from a security perspective they are better isolated
against each other. If one SCS is compromised it does not mean that
the others are compromised, too.

### (Independent) Scaling

Each SCS can run on one or multiple servers to deal with high
load. The SCS contains also the database and does not talk to other
SCS. So just scaling a single SCS is enough to support a larger number
of requests of a certain type.

### Replaceability

Each SCS can be replaced. Quite a few project try to replace legacy
systems. Those projects are usually quite complex and have a high
risk. Because each SCS can be replaced independently a migration is
much easier.

### Playground effect

It is much easier to try out new technologies and approaches. A
decision for a new technology can be limited to one SCS. So a
technology can be tried out with little risk but it will still run in
production. That avoids that the system will use outdated
technologies. Also migrating to a new technology is easier.

### Integration with Legacy

A legacy system might be enhanced with some SCS and slowly be
migrated - without touching a lot of the code. The integration of SCSs
is through the web. So it is easy to integrate the SCS with the legacy
system.

### Teams

An SCS might be a good unit of software for a team to work on. It
provides a business functionality so a team can work on stories for
just one SCS. That way SCS can influence the organization of the
project - according to [Conway's Law](http://www.melconway.com/Home/Conways_Law.html).

### Experience

We have seen this architecture work in many projects. We believe it
solves some of the current challenges in Software Development. See
also the [links](/links.html) - quite a few people find the
approach helpful.