![Client Logo](../../../../images/enigen.jpeg)
# Summary Statement of Architecture Work and Tailored Architecture
Project: Project Name
Client: Client Name

# Table of Contents
* Project Request and Background
  * Overarching Context
  * Specific Request
  *  Strategic Alignment
  * Suggested Simplifications
* Objectives and Scope
* Architecture Approach
  * Architecture Process
  * Architecture Content
* Relevant Methodologies and Industry Standards
* Support of the Enterprise Continuum
* Work Deliverables
  * Duration and Effort
* Risks and Mitigation
* Acceptance Criteria and Procedures
* Metrics and KPIs
* Approvals

# Project Request and Background
## Overarching Context
See [Architecture Definition document](../../architecture-definition-document) where this content 
has been moved and is currently up to date.

## Specific Request
Based on identified project [risks](../../risks/) the Architecture Advisory Board has requested
a learning spike that tests the hypothesis presented [here].() 

##  Strategic Alignment
![Client Target State Architecture].()

## Suggested Simplifications

* List 
 
# Objectives and Scope

# Architecture Approach
[ADD](../../architecture-definition-document)
[Architecture Framework](../../../../images/Agile-Transformation-Architecture-Framework.png)

## Architecture Process
Combining the Open Agile Architecture principles with TOGAF. The TOGAF architecture development method (ADM) defines a best-practice methodology for architecture development. However, not all phases are necessarily equally relevant to every project. The table below describes the usage of the ADM for this particular project.


 |  Phase  |  In / Out  |  Notes  | 
 |  -----  |  --------  |  -----  | 
 |  Preliminary  |   |   | 
 |  A – Architecture Vision  | IN  | _Consolidated into objectives of the PBusiness Hypothesis and Architecture Definition document_ | 
 |  B – Business Architecture  |  IN |  **Parallelized with C and D:**, _Operates in the domain_  | 
 |  C – Information Systems Architecture  |  IN  |  **Parallelized with B and D:**, _Operates in the domain_, _Aim to adhere to appropriate [Architectural Principles](../../architecture-principles/)_ |
 |  D – Technology Architecture  |   | **Parallelized with B and C:**, _Adheres to _  | 
 |  E – Opportunities and Solutions  | IN  | Focus on solutions architecture to satisfy testing the hypothesis | 
 |  F – Migration Planning  | IN  | _Focus on defining building blocks for enterprise solution, path to production and building blocks for a CI/CD deployment pipeline._ | 
 |  G – Implementation Governance  |   | Solution may use self-assessment based on architectural principles and focus on demonstrating conformance with specific principles.| 
 |  H – Architecture Change Management  | IN  | Architecture updates are permitted and should be documented through an approval history of pull-requests to architectural components and other artifacts. | 

This first cycle will set a baseline for the approach used with proof of concepts. Learnings 
may be shared through an accompanying document containing notes on those learnings.

## Architecture Content

The TOGAF Architecture Content Framework (ACF) provides a best-practice categorization of architecture content. However, not all items are necessarily equally relevant to every project. The table below describes the content areas relevant to this particular project.


 |  Content Area  |  In / Out  |  Notes  | 
 |  -----  |  --------  |  -----  |
 |  Architecture principles, vision, and requirements  |  IN |  Defined across [Architecture Principles](../../architecture-principles), [Architecture Definition document](../../architecture-definition-document) | 
 |  Business architecture  | IN  |  See high-level domain model in the [Architecture Definition document](../../architecture-definition-document)  | 
 |  Information systems architecture – Data  | IN  | Update this SoW if necessary. See also [Architecture Definition document](../../architecture-definition-document) The Architecture Committee recommend a Value (Outside-In) and Data-Driven approach.  |  
 |  Information systems architecture – Applications  |   |  Update this SoW if necessary. See also [Architecture Definition document](../../architecture-definition-document)  |  
 |  Technology architecture  | IN  |  Any updates to this document or the [Architecture Definition document](../../architecture-definition-document). Add a methodology and specification in the [Business Objectives](../../business-objectives) document. | 
 |  Architecture realization  | IN  | Complete software project with a working and specified API, proven using sound engineering and testing principles. In code/project documentation to also be supplied in the repository. Markdown to be provided with a roadmap to productionise or pivot, based on the learnings. | 

Key stakeholder concerns should be addressed and given priority, particularly in relation to response times, scalability, tolerance of system outages, and resilience under load.  

# Relevant Methodologies and Industry Standards
See [Architecture Principles](../../architecture-principles) and its specific principles for proofs of concept.

# Support of the Enterprise and Solution Continuum
Where possible, the solution should aim to either provide or facilitate the provision of solution and architecture building 
blocks that may benefit future proof of concepts and other engineering efforts.

Specifically, we would like the solution to produce:
* A testing strategy for proof of concepts.
* A test plan documented in the project that can inform other proofs of concepts.
* Demonstration of a CI/CD pattern that can be used for other projects.

# Work Deliverables

* A working implementation, tests with supporting documentation.
* Test Execution reports produced during continuous integration to demonstrate delivered behaviors.
* A presentation of the solution, proof of supported behavior, learnings, and future recommendations.

## Duration and Effort

Discuss with leadership team.

# Risks and Mitigation
See the [Risk Register](../../risks)

# Acceptance Criteria and Procedures
# Metrics and KPIs
Please define appropriately inline with the [Business Objectives](../../business-objectives/) and [Architecture Principles](../../architecture-principles).

# Approvals


