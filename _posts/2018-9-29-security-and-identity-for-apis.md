---
layout: post
title: Security and Identity For Apis?
permalink: :collection/:title
---

In a world of automation, how do we keep track of trust?
This topic has come up several times for me in the _hallway_ track at
[2018 RestFest Greenville](https://github.com/RESTFest/2018-Greenville)

| *Who Are You?* | *What Can You Do?* |

```yaml
- As A: System Integrator
- I Want a: Pattern to "Kick The Tires"
- So That I: know what damage is mine vs yours...
```

## Scenario:  Algorithim vs Training
[Mike Admunsen](https://github.com/RESTFest/2018-Greenville/wiki/Mike-Amundsen)
introduced me to this concept.  That in order to trust an
intelligent "thing" you need to know both
1. What the logic engine being used?
2. What is the data it was trained on?

It's not a new problem. We have the same challenge in choosing our human experts.

## Scenario: Physical Access Points
In my particular scenario,  I'm dealing with physical, wired points.  Every
thermistor, damper, valve is responding to local conditions, and to embedded
optimization routines.  _And any of these can be changed on the fly_

* Easy - I need to do _lots_ of these and fast
* Secure - Who installed and when?
* Permissions - Who is allowed to install what?

# Asked The Room

* Are you / How are you managing Identity?
* What are the identity brokers you trust?
* What anti-patterns for identity have you encountered?
* What barriers do we need to remove to move forward?

# They Responded

## Process Types
+ Tests + Assertions : don't use, work with entities that don't provide access to the Tests
+ A process that explicitly collects, publishes, links the evolution of the goals, schema, implementations

## Legacy + Internal
+ Implicit Trust no Security

## Brokered identity
+ JWT + Certs
+ Enterprise Legal, Contractual trust

## Broken Trust
Most recent Panera and credit cards published as a public resource file.
Too many developers still think that *obscure* urls are _safe_ and too much
data is getting exposed.
+ Scan ecosystems for secrets, PII

# Continue Learning
+ NordicApis
+ Troy Hunt
+ Web of Things
+ Verifiable Credentials
+ Bruce Schneier [Schneier on Security](https://www.schneier.com/)
