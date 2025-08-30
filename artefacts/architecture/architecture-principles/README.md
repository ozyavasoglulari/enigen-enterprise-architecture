![Client Logo](../../../images/enigen.jpeg)
# Architecture Principles

Too guide the architectural effort, the enterprise members have collaboratively
defined a set of architectural principles by domain. As with
any principles, these should be striven for in all project initiatives, 
all project initiatives should strive to meet them and justify any divergence.


# Summary of Principles

* A. Enterprise Architecture Principles
  * Principle A1: Primacy of Principles
  * Principle A2: Maximize Benefit to the Enterprise

* B. IT (System, Data, Solutions, Security, and Operations) Architecture Principles
  * Principle B1:  

* C. Architectural Methodology and Process Principles
  * Principle C1: A Centralized, Curated, Architecture Repository as the Source of Truth
     
     
# A. Enterprise Architecture Principles

## Principle A1: Primacy of Principles

**Statement:**

The principles stated here apply to all enterprise members, who we will collectively refer to as the **enterprise**.

**Rationale:** 

The only way we can provide a consistent and measurable level of quality information to decision-makers is if all Organisations abide by the principles.

**Implications:**

Without this principle, exclusions, favour itism, and inconsistency would rapidly undermine the management of and coherency
of architectural decisions.

Architecture initiatives will not begin until they are examined for compliance with the principles.
A conflict with a principle will be resolved by changing the framework of the initiative.

## Principle A2: Maximize Benefit to the Enterprise
 
**Statement**: 

Architecture and macro design decisions are made to provide maximum benefit to the enterprise as a whole in its efforts to maximize value impacted by those decisions.

**Rationale:**

This principle embodies "service above self." Decisions made from an enterprise-wide perspective have greater long-term 
value than decisions made from any particular Organisational perspective. Maximum return on investment requires architectural and design 
decisions to adhere to enterprise-wide drivers and priorities. No minority group will detract from the benefit of the whole. However, this principle will not preclude any minority group from getting its job done.

**Implications:**


# B. IT (System, Data, Solutions, Security and Operations) Architecture Principles


## Principle B1:  
 
**Statement**: 

**Rationale:**

**Implications:**

  
# C. Architectural Methodology and Process Principles
 
## Principle C1: Tailoring the TOGAF 9.2 ADM

**Statement**

The enterprise architecture will be shaped through customization and continuous improvement of an architecture framework 
tailored from TOGAF 10's ADM.

**Rationale:**

In order to provide a shared language and understanding of architecture, it is 
necessary to start from a well-defined and opinionated base. The OpenGroup's
TOGAF provides a framework which is centered around requirements management.

TOGAF includes governance and guidance that support specialization of a framework 
and methodology which can ensure the necessary levels or rigor when delivering 
functionality relating to patient safety, data privacy, overall information 
security, and desirable levels of correctness.  
 
**Implications:**

TOGAF's ADM includes governance and safeguards which are 
required to ensure an architecture capable of meeting ethical, business,
and state-level requirements around patient-centric software.

The enterprise architecture function will be responsible
for partnering with business, and technical stakeholders 
to agree on an architectural framework, which may also be modified
across projects and different business contexts.


## Principle C1: A Centralized, Curated, Architecture Repository as the Source of Truth

**Statement:**
All architecturally-relevant information should be made available 
by a central architecture repository, which is continuously curated
by, and under the custodianship of, the enterprise architecture function.

**Rationale:**

Where architecture artifacts are dispersed across multiple systems, it becomes
difficult, over time, for all partners to have a clear oversight of 
the current *relevant* state of the architecture and agreed-upon architectural 
framework and processes.

**Implications:**

A centralized architecture repository simplifies the problem of 
consolidating and curating all current architecture-level artifacts, decisions, and 
content in a landscape of constantly changing business and technical requirements.

## Principle C3: The Use of Agreed-Upon Open Agile Architecture Principles to Ensure High Standards

**Statement:**

Applying agreed-upon open standards and best practices can support the Organisation by providing the benefit of industry
learnings and expertise. 

**Rationale:** 

The principles outlined here build on industry best practices that have evolved alongside
supporting standards and guidelines. Using associated standards can support the benefits 
of the principles we align with.

**Implications:**

We will encourage and support, at least, the following open standards and best practice architectural patterns. All 
designs and architectures should be designed, where appropriate, to support extensions. 

**Initiatives are advised to document how their solutions either support these standards or are designed to be extended to support them.**

[OAA-Architecture Design](../../../images/Agile-Transformation-Architecture-Framework.png)

* Event-driven architectures
  * Event sourcing
* Microservices architectures
  * OpenAPI specification of service contracts
  * Service meshes
     * Service observability
     * Service monitoring
     * Service discovery
     * Service integration visibility
  * Deployment through containerized, immutable, and repeatable infrastructure
* Domain-driven design
* Behavior-driven development
  * To ensure the correctness of expected patient-centric outcomes.
  * To support an aligning development with a ubiquitous language.
* Fault tolerance and design for long-term chaos engineering.
* OpenID Connect integration with state-run patient identity providers.
* Technology selection:
  * Should favour OCI and Oracle SaaS languages due to enterise guidelines.  
* Documentation:
  * Should favour Git Repository for source code and markdown or ASCIIdoc for project-level documentation.

As this defines a target state, it is acceptable to compromise on these, but such compromises should be documented and justified. 

## Principle C4: Fostering a Learning Culture With Proof of Concepts, Prototypes, and Spikes

**Statement:**
 
The enterprise encourages learning-centric implementations that reduce risk, validate assumptions, and 
invest in the learning required to evolve the platform responsibly.

**Rationale:**
The enterprise collectively encourages the use of proof of concepts, spikes, and prototypes, as well as 
other investigative avenues of pursuit in order to *safely fail-fast* around
areas where there is insufficient information available to understand the risk of making 
 specific production-level design or implementation decisions. 
 
The cost of investing in learning efforts to reduce risk is encouraged across the 
enterprise as a means of protecting the interests of patients, partners, and the enterprise.

**Implications:**

The enterprise partners collectively agree to stimulate a culture
 of evidence-based, and learning-centric, decision making. 
 
In so doing, the following exceptions and considerations should apply:

**i) Provide a hypothesis for every learning**

* All learning related implementations should be accompanied with a *hypothesis* defining the 
desired learning and how to measure whether that learning outcome has been achieved.


**ii) Isolate proofs of concepts from production data and systems**

* Action should be taken to mitigate or eliminate the risk of impacting patients where there is risk or uncertainty of
causing harm to the patient or enterprise. For example, learning may be conducted in isolation within a contrived environment to avoid impacting production systems.

**Use fabricated or anonymized data** 

* Patient data should be protected from high-risk learning activities which 
may impact data security or patient care. Early proof of concepts 
may use anonymized or fabricated data where possible.

**iii) Relax compliance but consider the consequence of doing so**

* Governance standards and levels of compliance may be 
relaxed where steps are taken to protect production systems and patient data. For example, proof of concepts
isolated from real patient data and production systems are not required to
conform to external standards or all enterprise governance around its ability to be released. 
* Where standards and governance are not fully adhered to, 
implementers and designers should recognize the need to 
consider how such prototypes or learning-focused implementations 
may feed their lessons into final producible implementations.
* It is strongly discouraged to produce prototypes directly, but 
 instead ensure that designs account for the side-effects of 
 the production that may invalidate any leanings. Eg., Omitting security concerns
 or expected data-volume may result in performance penalties which 
 invalidate learnings from an unscalable prototype. 
* Performance testing of prototypes and learning-centric implementations 
should demonstrate the key algorithms that form part of that learning scale.


**iv) Basic engineering, delivery, and testing principles are not to be relaxed for the solution architecture of proofs of concepts**

Proof of concepts should specifically aim to adhere to the following principles:
* Principle B1: Business continuity of patient critical systems
* Principle B2: Clarity through a Fine Grain Separation of Concerns
* Principle B3: Continuous Integration and Delivery
* Principle B4: Early Comprehensive and Appropriate Automated Tests

**v) Test plans as a tool for communicating requirements**
* Deliverables with self-documented test plans are preferred over externally documented test plans.
* Proof of concepts should have test plans describing how the product should behave.
* Test plans should utilize BDD (See C3) to describe business acceptance criteria that are in scope.
* Test plans should use the shared language of the business and be understandable by 
 technical and non-technical partners. 

**vi) Test execution reports as documentation for supported behavior**

To support the visibility of supported behavior, continuous learning, and transparency around software state: 
* Architecture should have CI pipelines that run tests and produce test execution reports.
* CI environments should allow software owners to inspect past runs and degradations of the build*, which may affect any learnings from the hypothesis in Line with B3.

  
 
