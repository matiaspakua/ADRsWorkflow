# First-Decision

* Status: proposed
* Date: 2021-08-24

Technical Story: ADR-001

## Context and Problem Statement

Select the proper structure for the ADR repository.

## Considered Options

* ADR Github
* MADR
* Combine MADR and PlantUML

## Decision Outcome

Chosen option: "Combine MADR and PlantUML", because Combines the best soluctions.

### Positive Consequences

* Best Organization
* Clarity

### Negative Consequences

* Needs an Example Diagram

### Example Diagram:
![your-UML-diagram-name](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/matiaspakua/ADRsWorkflow/main/docs/adr/0001-diagrams/first-diagram.iuml)


```plantuml
actor Promoter
actor Entrant

Promoter --> (Create Event)
Promoter -> (Attend Event)

Entrant --> (Find Event)
(Attend Event) <- Entrant

(Attend Event) <.. (Create Member)  : <<include>>
@enduml
```