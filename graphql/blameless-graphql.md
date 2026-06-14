# Blameless SRE GraphQL Schema

## Overview

Blameless is an SRE and incident management platform purpose-built for reliability engineering teams. It covers the full incident lifecycle — detection, response, retrospectives, and continuous improvement through SLOs and error budgets. This conceptual GraphQL schema models the Blameless platform domain as described in the Blameless public documentation at https://docs.blameless.com.

## Schema Source

This schema is a conceptual GraphQL representation derived from the Blameless REST API surface area and public product documentation. It is not an officially published GraphQL endpoint by Blameless. The schema serves as a structured reference for understanding the Blameless data model and relationships.

Reference: https://blameless.com/docs/api/

## Core Domain Areas

### Incident Management

The Incident domain covers the entire lifecycle of a reliability event from detection through resolution. Key types include `Incident`, `IncidentDetails`, `IncidentStatus`, `IncidentSeverity`, `IncidentTag`, `IncidentMilestone`, `IncidentEnvironment`, `IncidentOwner`, `IncidentReporter`, and `IncidentTimestamp`. Incidents link to SLOs, timelines, actions, and retrospectives.

### Timeline and Actions

The timeline captures the sequence of events during an incident. `Timeline` holds a list of `TimelineEntry` records. `Action` types track remediation tasks with status (`ActionStatus`) and ownership (`ActionOwner`).

### Retrospectives

After resolution, teams conduct blameless post-mortems. `Retrospective` contains `RetroSection` groupings, individual `RetroItem` findings, and `RetroFollowUp` tasks that feed back into the action backlog.

### SLOs and Error Budgets

Service Level Objectives are a central reliability construct. `SLO` and `SLODetails` define the objective. `SLOTarget` specifies the threshold. `SLOBudget` and `ErrorBudget` quantify remaining reliability margin. `BudgetBurn` and `BurnRate` track consumption velocity, and `BurnAlert` fires when burn exceeds acceptable thresholds.

### SLIs and Data Sources

`SLI` and `SLIDetails` define the measurement. `SLIDataSource` identifies the upstream metrics system (Prometheus, Datadog, etc.) that feeds the SLI calculation.

### Alerting

`Alert`, `AlertSource`, and `AlertPriority` represent inbound signals from monitoring systems that may trigger incidents.

### Users, Teams, and On-Call

`User` and `Team` model the people involved. `Schedule` and `EscalationPolicy` cover on-call rotation and escalation paths.

### Workflow and Automation

`WorkflowTemplate` and `WorkflowTrigger` define automated runbooks and the conditions that activate them.

### Integrations and Access

`Integration` represents third-party tool connections. `Webhook` models outbound event subscriptions. `APIKey` and `Token` represent authentication credentials for API access.

## Named Types (56 total)

| Type | Category |
|---|---|
| Incident | Incident |
| IncidentDetails | Incident |
| IncidentStatus | Incident |
| IncidentSeverity | Incident |
| IncidentTag | Incident |
| IncidentMilestone | Incident |
| IncidentEnvironment | Incident |
| IncidentOwner | Incident |
| IncidentReporter | Incident |
| IncidentTimestamp | Incident |
| IncidentSLO | Incident |
| Timeline | Timeline |
| TimelineEntry | Timeline |
| Action | Action |
| ActionStatus | Action |
| ActionOwner | Action |
| Retrospective | Retrospective |
| RetroSection | Retrospective |
| RetroItem | Retrospective |
| RetroFollowUp | Retrospective |
| SLO | SLO |
| SLODetails | SLO |
| SLOTarget | SLO |
| SLOBudget | SLO |
| ErrorBudget | SLO |
| BudgetBurn | SLO |
| BurnRate | SLO |
| BurnAlert | SLO |
| SLI | SLI |
| SLIDetails | SLI |
| SLIDataSource | SLI |
| Alert | Alert |
| AlertSource | Alert |
| AlertPriority | Alert |
| User | People |
| Team | People |
| Schedule | On-Call |
| EscalationPolicy | On-Call |
| WorkflowTemplate | Workflow |
| WorkflowTrigger | Workflow |
| Integration | Integration |
| Webhook | Integration |
| APIKey | Access |
| Token | Access |
| Query | Root |
| Mutation | Root |
| IncidentInput | Input |
| ActionInput | Input |
| RetroItemInput | Input |
| SLOInput | Input |
| SLIInput | Input |
| AlertInput | Input |
| WebhookInput | Input |
| IncidentConnection | Pagination |
| PageInfo | Pagination |
| SLOConnection | Pagination |

## Query Examples

### List recent incidents

```graphql
query RecentIncidents {
  incidents(first: 10, status: ACTIVE) {
    edges {
      node {
        id
        title
        severity { level label }
        status { name }
        owner { user { name email } }
        createdAt
      }
    }
    pageInfo { hasNextPage endCursor }
  }
}
```

### Get SLO error budget

```graphql
query SLOErrorBudget($sloId: ID!) {
  slo(id: $sloId) {
    id
    name
    target { percentage window }
    budget {
      remaining
      consumed
      errorBudget { minutesRemaining percentage }
    }
    burnAlerts { id threshold triggered }
  }
}
```

### Create an incident

```graphql
mutation CreateIncident($input: IncidentInput!) {
  createIncident(input: $input) {
    id
    title
    severity { level }
    status { name }
    createdAt
  }
}
```
