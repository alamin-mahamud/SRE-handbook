# SRE-handbook

## What is SRE
* `S` stands for `site` | `system` | `software`
* `R` stands for `reliability` | `resilience`
* `E` stands for `engineering` | `engineer`
* **Realm** - anything as a service falls into the realm of SRE
  * `IaaS`
  * `PaaS`
  * `NaaS`
  * `SaaS`
  
* To make a service more maintaianable, reliable SRE uses some indicators and objectives to hit the target
  * **Service Level Indicators**
  * **Service Level Objectives**

## Major Areas of expertise
* Release Engineering
* Change Management
* Monitoring and Observability
* Managing and Learning From Incidents
* Self-Service Automation
* Troubleshooting
* Performance
* The use of deliberate adversity (chaos engineering)

SRE works to help an organisation sustainably achieve the appropriate level of reliability for its services by implementing and continually improving data-informed production feedback loops to balance availability, performance and agility.

## Production Feedback Loops
* Feedback does not work if you don't put care, feeling, attention and necessary action for that
* Feedback at its core is a communication with sociotechnical system
  * Technical Level - Threads, Processes, Servers and Services
  * Social Level - Team, People, Product, Companies, Regions or any other level of communication

### Data Informed Feedback
* Feedback should be based on data not opinions
* For which time some incidents are happening and what was the condition/context of that environment at that moment, is a very good metric for most of the cases.
* what constraints were missing, that could not handle the incident
* Changes in the environment or better understandings of the dynamics of a system can lead to valid technical arguments about whether a measurement / strategy is accurate or effective in particular context.

### Mechanism to track and manage the outage budget
* Service Level Indicators - SLI
  * What you measure and where the measurement is taken?
  * Can we recreate the exact environment and recreate the issue, based on the input we have right now?
  * what data should we look at so that we can make sure this never happens in the future?
* Service Level Objective - SLO
  * The goal of threshold of acceptable values for the SLI within a given time period
  
## Incidents Response

* SREs are frequently at the forefront to remediate them, because of their commitment to learn from failures and reduce outage durations
* **Emphasis on blameless postmortem**
* SRE team, must need to work on projects that will, **make tomorrow better than today**.

## Where did SRE Came From?
* SRE is an outgrowth of `always on` world of online services.
* TDT - Time to detect something
* TTR - Time to Respond
* TTM - Time to Mitigate

## Distinction betewen DevOps and SRE

* DevOps - focuses on engineering continuous delivery to the **point of deployment**
  * devops makes sure that whatever new features are coming should be able to continuously delivered in a smooth manner
* SRE - focuses on engineering continuous operation to the point of **customer consumption**
  * priority for SRE teams is on the **delivery of value to end users**
  * makes sure the application will remain secure, reliable and fault-tolerant and most importantly does it's job what it's supposed to do, solve business problem and birng value to client/customer

* Principles are Easy, But Applications are Hard. **A minute to learn, but a lifetime to master**

## Understanding the SRE Role

* `Culture` - having a culture where people can experiment new things. 
  * it means the way a company does things
* `Capabilities` - combination of skill, technology and knowledge that the firm execute specific activities and innovation process
  * Broad understanding of computer system dynamics - especially distributed systems
  * Effective SRE's zoom out to deal with system level interrelationships and to zoom in, as needed to debug the bit level intricaceis of networking or memory-usage pattern
* `Configuration` - structures of organization, who bears responsibility for achieving targets and how success is measured
* Adequate Feedback loops help us to avoid cascading problems and the so-called `dark` debt within distributed systems

* During Jan-Feb When all the US Govt Dept was closed. All the Govt sites were getting denial of service because TLS Certificates were not rotated. If someone was there he/she would have rotated the certificates. But SRE would make sure this would be rotated every time automatically w/o human intervention.

## Implementing SRE

* New/Fresh Project —> GreenField Project
* Existing/Old Project —> BrownField Project
* Hierarchy of Reliability
  * Food, Sleep, Family
  * Metrics
  * Monitoring
  * Incident Response
  * Postmortem / Root Cause Analysis
  * Testing and Release Procedures
  * Capacity Planning
  * Development
  * Product

The SRE is **not the ops person** for the team. It is easy for everyone to just hand off deployments, configuration management, etc. to this one individual. But if that happens we already implemented the **classic ops** just at a smaller scale. 

The SRE is there to enable & empower every other engineer on the team. Each engineeri is responsible for deploying their own code and managing their own configurations. 

They are there to make the jobs of every other engineer easier and faster

## Case Study - LinkedIn's SRE Team's Focus
* Site up and secure is the prime directive
* everyone in the engineering organization should be able to safely deploy code
* operations is an engineering problem

## AntiPatterns of SRE

* changing the name of any existing team (usually "ops") to "SRE" without making the organizational adjustments required to enable them to do meaningful development work.
* using the SRE team to shield devs from the pain of how their services really function in production
* Failing to contain interrupts
* Attempting to do SRE Project work without the same support (such as project managers, technical writers etc.)
* Valuing incident response heroics over prudent design and preventative planning
* Implementing processes or systems that slow down the delivery of value to customers w/o incontrovertible benefit
* Building a "gatekeeper" team that functions as a chokepoint
* Static or ill-considered SLOs


  
