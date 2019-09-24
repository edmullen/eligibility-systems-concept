[Return to introduction](index.md)

# _Strength #5:_ State staff have tools that empower them to deliver excellent service and achieve their mission

The tools eligibility workers, their managers, and those who lead public assistance administration in states use should empower these civil servants to serve their clients more efficiently and effectively. Their tools should:

- be intuitive and smart
- drive mission success
- reduce uncertainty in the process
- get people enrolled and receiving benefits quickly
- be more holistically integrated
- make data intelligence easy, allowing the programs to evolve and improve.

**All too often, existing systems that workers must use are outdated, laborious, and hard to use.** States don’t have the resources or expertise to make these systems modern, usable, and empowering. It’s unreasonable to ask states to continuously improve their systems based on continuous user feedback loops with their current mix of staffing and skill. And we’ve learned incumbent vendors are not incentivized to build great experiences for workers.

**It doesn’t have to be this way.** The tools workers use _can_ make the worker experience more gratifying and effective, can make the management of state teams easier, and can make needed reporting simple. But it requires new operating models, more de-coupling of pieces, more integrated, shared services, and ongoing support and development.

## A concept for a state worker app

I have mocked up a concept for what an empowering worker experience could look like.  It illustrates how applicant data for multiple users could be collected, reviewed, and processed within an interface designed specifically for power users (as opposed to the occasional nature of individual client users.).  

**This prototype is incomplete.** You'll find dead-ends or screens that are empty. Follow the blinking blue dots to find the fields you can click on. Submitting a new blank application is the workflow I focused on mostly.

<span style="background-color:#ccf0ff;text-align:center;display:block;color:white;font-size:1.75em;padding-left:1em;padding-right:1em;padding-top:.5em;padding-bottom:.5em;margin-top:1em;margin-bottom:1em;font-weight:bold"><a href="https://gsa.invisionapp.com/share/32QAEWUR9HG">View the prototype</a></span>

> **I would LOVE to further explore this idea.** If you would too, I'd love to speak with you. As my term at 18F is winding down, I am exploring what my next adventure should be, and I'd love to find ways to build empowering experiences for eligibility workers.

This work is [open source](LICENSE.md). Here's the [Sketch file](/concept_assets/eligibility-system-concept.sketch) used to create the prototype.

## High level workflow

The diagram below describes the workflow of an applicant’s data moving through the loosely-coupled system that includes the state integrated eligibility & enrollment app, the data storage, and the rules services.

Most of the activities described take place in the state app. Use the cross-references to jump to the screens in the prototype to see how these pieces could function.

![Illustration visualizing the steps below](/concept_assets/concept-workflow.png)

1. **Multiple pathways to apply** - Multiple ways to apply exist by different parties. Clients can do it on their own or with the help of eligibility workers or assistors.
2. **Data intake** - All the data a client needs to submit across the programs they are applying for is gathered at once in a single, merged intake form. [See _Applicant data submission_](data.md)
3. **People-centric data** - The client’s data, not yet applied to a specific program, is saved into a modern, non-proprietary database that’s structured around the person.
4. **Applications populated** - The client’s data is used to populate applications for each program they are applying to.
5. **Eligibility rules applied** - The E&E system sends anonymized application data to the eligibility web services for each program which analyze it for eligibility and send responses back to the E&E system. [See _Eligibility policy as code_](eligibility-policy.md)
6. **Eligibility worker review** - Eligibility workers review applicant data, get clarifications from client as needed, advise on additional program eligibility.
7. **Eligibility workers make determinations** - Eligibility workers make the final call on eligibility determinations.
8. **Benefits are issued** - Once a determination has been made, benefits are issued. Program maintenance activities happen after this: life changes, recertifications, etc. (not shown).

## The Worker experiences

You can [navigate around the prototype](https://gsa.invisionapp.com/share/32QAEWUR9HG), or jump into specific sections from the links below. (You may need to scroll to get to the intended section of the page due to prototype limitations.)

<span style="background-color:#ccf0ff;text-align:center;display:block;color:white;font-size:1.75em;padding-left:1em;padding-right:1em;padding-top:.5em;padding-bottom:.5em;margin-top:1em;margin-bottom:1em;font-weight:bold"><a href="https://gsa.invisionapp.com/share/32QAEWUR9HG">View the prototype</a></span>

#### Entry

The entry is focused on helping the worker get right into doing the work they need to. Search is the primary, persistent method for finding the people who they are trying to help. The homepage could feature key actions and highlight urgent wok assigned to them.

- [Homepage](https://gsa.invisionapp.com/share/32QAEWUR9HG#/screens/343810595)
- [Search](https://gsa.invisionapp.com/share/32QAEWUR9HG#/screens/343810596)

#### People

The experience, and data, is oriented around people. People are connected to other people as families or participants in applications to programs together. Workers could identify likely addition program eligibility and take action.

![Illustration showing a person as the central data point, with other people, applications to programs, and programs themselves connected](/concept_assets/concept-person.png)

- [Person record](https://gsa.invisionapp.com/share/32QAEWUR9HG#/screens/343810613)

#### Worker-submitted applicant data

While applicants would have multiple ways to apply, worker-submitted applicant data collection would be optimized for applying to multiple programs at once in a streamlined experience. The system could also suggested other programs the applicants are likely eligible for based on submitted information.

- [Blank applicant, joint intake](https://gsa.invisionapp.com/share/32QAEWUR9HG#/screens/343810598)
- [Primary individual](https://gsa.invisionapp.com/share/32QAEWUR9HG#/screens/343810599)
- [Households](https://gsa.invisionapp.com/share/32QAEWUR9HG#/screens/343810601)
- [People questions](https://gsa.invisionapp.com/share/32QAEWUR9HG#/screens/343810602)
- [Money](bit.ly/2TGkv9E)
- [Expenses, Applications](https://gsa.invisionapp.com/share/32QAEWUR9HG#/screens/343810605)

#### Data has been submitted

Once the applicant’s data is submitted (either through worker app, self-submission, or other routes), the data is used to populate an official application for benefits from each program the applicant is applying to. From this point, eligibility workers have a number of actions to take.

- [Confirmation screen (incomplete)](https://gsa.invisionapp.com/share/32QAEWUR9HG#/screens/343810606)
- [Application (incomplete)](https://gsa.invisionapp.com/share/32QAEWUR9HG#/screens/343810614)

#### Review

Application data that must be verified can be reviewed once across all applications. Policy that makes this difficult should be revised. Any verifications that can be automated should be.

- [Review](bit.ly/2u9iR1d)

#### Issuance (incomplete)

Issuance should be automated when possible, easily trackable. (This area is less known to me at this point.)

#### Maintenance (incomplete)

As much of the recertification process that can be automated should be. Other needed actions should be signaled clearly.

## The Manager experience

#### Empowering managers

This area needs to be fleshed out further. It should provide managers with visibility into the current operations of their workforce. This would include visibility into the workload, useful metrics to let them know how they are doing, access to third-party tools powered by system data, and more.

## The Director experience

#### Empowering directors

This area needs to be fleshed out further. State directors need to be empowered with on-demand tools that show the current status of state operations, access to neccessary data, and one-click compliance with federal data reporting requirements.

<span style="background-color:#ccf0ff;text-align:center;display:block;color:white;font-size:1.75em;padding-left:1em;padding-right:1em;padding-top:.5em;padding-bottom:.5em;margin-top:1em;margin-bottom:1em;font-weight:bold"><a href="https://gsa.invisionapp.com/share/32QAEWUR9HG">View the prototype</a></span>

---

### [Next](incremental.md)
