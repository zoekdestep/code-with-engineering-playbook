# Security testing

Software systems are susceptible to malicious attacks; the impact of such security breaches can be
[costly to businesses and their customers](https://en.wikipedia.org/wiki/List_of_data_breaches).
Security testing is a mechanism to detect security vulnerabilities to be fixed and to prevent exposure when attacked.

This document discusses security testing and provides insights on how to applying it to your software.

<!-- markdownlint-disable -->
## Why security testing?
<!-- markdownlint-restore -->

Software almost literally exists in every aspect of our lives, from entertainment to critical software that helps protect human life.
As a side-effect of its wide-spread, malicious attacks are always on the raise to exploit software systems.
The impact of such attacks can be costly on the business,
as they may lead to the loss of customer trust, and as a consequence, loss in revenue.

The software needs to be assessed by the software developers to ensure it is protected against such attacks.

## Introduction to security testing

The key idea behind security testing is to vet a software system to detect and address security vulnerabilities as part of the software development life-cycle (SDLC).
Addressing a vulnerability can take various forms, from modifying the system to eliminate it, to acknowledging it and identifying a mitigation plan to be executed if it was exploited.

Security is an ongoing concern that needs to be considered throughout the SDLC of a product from inception till deprecation.
Applying this would help cost-effectively produce more secure software,
pushing the security until a later phase might be costly as it may require major re-arch and refactoring of the system.

![Security testing process](./Docs/SDLC_w_SC.png)

The figure above shows what a typical SDLC looks like, the lower chart shows potential security considerations to keep in mind in each SDLC phase.

* **Requirement gathering phase:** security requirements should be considered as the product is being defined (i.e., securing sensitive data).
* **Design phase:** this phase is influenced significantly by the security requirements as those
would set constraints on the design and guide technology choices. A common task within the design phase is [risk assessment and threat modeling](https://owasp.org/www-project-web-security-testing-guide/v41/2-Introduction/README.html#threat-modeling) to help identify risks that need to be mitigated during implementation and vetted during the verification phase.
* **Implementation phase:** this phase needs to address identified risks from the design phase. It also needs to adhere to the security best practices during implementation to guard against common pitfalls and vulnerabilities upfront.
* **Verification phase:** this phase performs various tests to vet the software system for common attack patterns and the identified risks in the design phase.
* **Release and Maintenance:** security is an ongoing concern that needs to be revisited constantly to ensure that the software system is protected.

The rest of this article will focus on the verification phase.

## Performing security testing

The following is a list of common categories for security tests:

* **_Manual inspection_**: in this category the security tester performs manual review of the implemented architecture to inspect changes from the original design, interview developers on flows and decision choices, and assess the architecture for new risks. The the developer would review the implementation decision made, assess risk,  of the code to ensure it
* **_Vulnerability detection tools_**: this kind of testing relies on static and dynamic code analysis techniques to evaluate the software code base for common vulnerabilities or attack patterns.
* **_Penetration testing_**: to affirm that the software has the right mechanisms in place to test against attackers, this kind of testing actually attacks the software with the intent of breaking through and breaching the software! If it succeeds, then it had identified a vulnerability in the system than needs to be addressed.
* **_Penetration testing_**:

## Examples/Case studies

TBD

## Resources

* [Learn more about security in the security playbook](../../security/README.md).
* [A good read on how to design secure cloud solutions on Azure](https://docs.microsoft.com/en-us/azure/security/develop/secure-design)
* [Azure security documentation](https://docs.microsoft.com/en-us/azure/security/)
* [Where can I learn more about threat modeling?](https://martinfowler.com/articles/agile-threat-modelling.html#:~:text=Threat%20modelling%20is%20a%20risk,to%20build%20security%20into%20software)

## References

* This article
<https://owasp.org/www-project-web-security-testing-guide/v41/2-Introduction/README.html#threat-modeling>

<https://www.guru99.com/what-is-security-testing.html>

<https://www.hack2secure.com/blogs/crucial-stages-of-software-security-testing-life-cycle>

<http://softwaretestingfundamentals.com/security-testing/>

<https://medium.com/@mprakash72/security-testing-in-development-cycle-8047e60886d>

* **Identifying** security vulnerabilities within the system that would put the system at risk of an attack.
* **Mitigating** the identified vulnerabilities either by fixing/eliminating them or by acknowledging them and owning the risk of them being exploited.
* **Verifying** that the software is protected against malicious attacks, this is done by attacking the software in an attempt to breach it.

drive what technology choices to make and what risks might exist that need to be addressed.
As part of the design phase, the designer should consider
[threat modeling](https://owasp.org/www-project-web-security-testing-guide/v41/2-Introduction/README.html#threat-modeling) for the system and plan for security testing.
