---
status: Proposed
date: 24-04-2026
deciders: PatientPingeling
---

# AD: Technologie stack

## Context en Probleembeschrijving

Jullie leggen vast met welke taal, framework, berichtenwachtrij, opslag en monitoringtooling de module gebouwd word. Per keuze beargumenteren jullie waarom deze technologie past bij de eisen van de opdracht én bij de capaciteiten van het team.

Met welke taal, framework, berichtenwachtrij, opslag en monitoringtooling wordt de module gebouwd?

## Beslissingsfactoren

- Reduce complexity
- Improve maintainability
- Support scalability

## Overwogen Opties

1. C#

## Resultaten

We decided to use **C#**.

Wij kozen voor C#/dotnet als technologie, omdat dit erg veel overeenkomt met de Java programmeertaal. Wij hebben niet voor Java gekozen, omdat de message broker "RabbitMQ" niet kijkt naar de taal waarmee de data verstuurd wordt en wij als team sterker zijn met C#. C# is moderner dan het aankomt op async/await en heeft een sterk ecosysteem ook voor het gebruik van RabbitMQ.

### Gevolgen

- Goed, omdat de module volledig afgeschermd is van de hoofdapplicatie en zeer schaalbaar is.
- Good, omdat de taal zeer modern is met een groot ecosysteem.
- Slecht, omdat developers met verschillende stacks moeten werken. Er worden 2 verschillende talen en frameworks gebruikt bij het werken aan de notificatie module met OpenMRS en C#.

## Meer Informatie

- Module developer documentation, how to use our message broker: https://openmrs.atlassian.net/wiki/spaces/docs/pages/25462172/For+Module+Developers
