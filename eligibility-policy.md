[Return to introduction](index.md)

_Note: This repository represents my personal work, done in my personal time and capacity. It is not representative of GSA (my employer at the time of publishing)._

# _Strength #2:_ Eligibility policy is delivered as functional code.

Federal programs that define who is entitled to receive benefits should provide official implementations of eligibility criteria in code that states and others can integrate into their eligibility systems via APIs. No longer should state after state need to hire vendors to interpret, build, and maintain the same business logic. That approach is expensive, duplicative, error-prone, risky, and leads to vendor lock-in.

Creating an ecosystem of Eligibility APIs would dramatically simplify modernization efforts and move states towards simpler, easier-to-modernize eligibility systems. Potentially, even simple commodity case management systems could replace today's custom systems.

![Diagram visualizing the following five aspects of Eligibility APIs.](/concept_assets/eligibility_apis.png)

1. State collects the data needed for multiple programs at once.
2. The collected data is used to concurrently apply to programs separately.
3. Anonymous application data is sent over the internet to the program’s rules service.
4. The rules service evaluates the data against the federal and state eligibility rules and instantly sends back a pass or fail message that’s used by states to help make eligibility determinations.
5. The rules services are owned and operated by the federal program agencies. The rules services are official translations of policy into code. They are configurable by states, accommodating all state options and variations. These official rules avoid all the interpretation, translation, and implementation challenges that happen when states and vendors try to take prose policy and build systems that make it actionable.

It’s not enough to build Eligibility APIs as model implementations or as “screeners” to indicate potential eligibility. Eligibility APIs should be owned and operated by the federal programs and be considered policy-as-code; business logic those sending requests can trust as official eligibility recommendations.  

Others have advocated for similar approaches previously. In section 1561, the Affordable Care Act called for "interoperable and secure standards and protocols that facilitate enrollment of individuals in Federal and State health and human services programs". The HIT Policy Committee and the HIT Standards Committee [made the following recommendations](https://www.healthit.gov/sites/default/files/rules-regulation/aca-1561-recommendations-final2.pdf),

> _Recommendation 3.1:_ Federal agencies and States should express business rules using a consistent, technology-neutral standard format, congruent with the core data elements identified through the NIEM process. Upon identification of a consistent standard, Federal agencies and States should clearly and unambiguously express their business rules (outside of the transactional systems).

> _Recommendation 3.2:_  To allow for the open and collaborative exchange of information and innovation, we recommend the Federal government maintain a repository of business rules needed to administer Affordable Care Act health insurance coverage options (including Medicaid and CHIP), which may include an open source forum for documenting and displaying eligibility, entitlement and enrollment business rules to developers who build systems and the public in standards-based and human-readable formats...To allow for seamless integration of all health and human services programs, business rules for other health and human services programs such as SNAP and TANF should be added to the repository over
time.

[MAGI in the Cloud](https://www.medicaideligibilityapi.org) made “MAGI Medicaid” eligibility criteria, new criteria for determining Medicaid eligibility introduced in the Affordable Care Act, available via API starting back in 2013. Several states have used the service as part of their eligibility process. But when MAGI in the Cloud launched, most states establishing their own exchanges felt optimistic that the monolithic vendor solutions would suffice. That turned out not to be true.

![Eligibility APIs Initiative logo](/concept_assets/eligibility_apis_logo.png)

18F has been pursuing this concept through four rounds of 10x funding. See the [Eligibility API Initiative](https://github.com/18F/eligibility-rules-service/blob/master/README.md) for more info.

---

### [Next](data.md)
