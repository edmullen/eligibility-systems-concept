[Return to introduction](index.md)

_Note: This repository represents my personal work, done in my personal time and capacity. It is not representative of GSA (my employer at the time of publishing)._

# _Strength #1:_ A loosely-coupled ecosystem of state, federal, and commodity software products, web services and data powers federal/state safety net programs.

The current distribution of technology responsibilities between federal and state safety net agencies needs to change. Today's rigid separation between federal program/policy design and state technical implementation has bred an ecosystem characterized by stagnation, duplicative effort, system failures, waste, and poor outcomes for our neighbors involved at each level.

**We should move towards a loosely-coupled ecosystem built of state, federal, and private sector components, each with clearly defined purposes and appropriate ownership, speaking to each other through web services, and assembled into solutions that empower their users while increasing effectiveness and efficiency.**

This shift will force us to challenge our assumptions around what states should be responsible for and what feds can provide for use.

## Current assumptions of responsibility

Many of the key programs that make up our social safety net are joint federal/state programs. The federal government created and defined the programs, established broad requirements, operational models, state responsibilities, distribution of partial funding, oversight responsibility, data collection, claims models, and more. States administer the programs, define the state's implementation approach, run program in the state, comply with federal requirements, and directly serve the public.

When it comes to the technology systems that make programs work, the feds define a broad array of things the systems should do including how eligibility determinations should be made, data that must be submitted back to the federal government, security requirements, even system architectures and software life cycles. States are expected to buy, build, and operate technology that adheres to these prescriptions. Their adherence to these prescriptions is enforced through funding requests and compliance actions.

Each state, from CA with its 40 million residents to Wyoming with its 600,000, is expected to stand up and run systems that do roughly the same thing. These are generally "_state_ systems" that assume all functionality is the full responsibility of the state to create. The similarity between state systems is often masked by state implementation choices and homespun workflows. State agencies typically struggling with resource issues and diminished technical expertise don't have the personnel to develop these mission-critical systems in-house. They rely on a relatively small number of incumbent vendors who benefit from the disempowered position of states.

**The result is a pattern of failed IT projects that impact both the lives of those served by the programs and diminished public belief in the ability of the programs' ability to deliver on their missions.**

## Redistributing responsibilities
Our assumed distribution of responsibility—that each state needs to build or buy fully self-contained systems that do everything—does not need to continue. Modern software development practices tend to favor "maximizing work not done": adopting commodity solutions, utilizing platform capabilities whenever available, and reducing the footprint of unique homegrown software as much as possible.

**Modern software development methods offer the opportunity to re-distribute the technical responsibilities that make up the systems used to operate our safety net programs.** Habit more than technical or policy constraints perpetuate this status quo. We frequently use the word _system_ to refer to monolithic things, when really a system is a set of things working together. It's time to look at the various pieces within our state systems, identify opportunities to pull out common aspects, and seek new arrangements that allow the whole of the ecosystem to benefit from shared use.

**It's time to build towards a _loosely-coupled ecosystem_.** This loosely-coupled ecosystem would have new pieces that are operated by the federal government that states can integrate with and use. It would utilize inexpensive commodity tools offered broadly in the private sector. Microservices from companies would be employed where appropriate to provide functionality the companies are uniquely positioned to offer. Custom development would be reserved for situations where other options are not available. Application programming interfaces (APIs) would assemble all the pieces into user-centric products which would be deployed on cloud infrastructure.

It will take time for all the pieces to emerge. Subsequent pages in this piece describe some aspects of this loosely-coupled future, but this is just a start:

- [APIs for eligibility policy](eligibility-policy.md)
- [Progressive applicant data submission](data.md)
- [Client experiences are intuitive, appropriate, and empowering](client-experiences.md)
- [Worker tools that empower excellent service delivery](state-staff.md)
- [Incremental legacy transformation](incremental.md)


---

### [Next](eligibility-policy.md)
