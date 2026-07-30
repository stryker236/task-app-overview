# Task App

Task App is an evolving personal productivity agent designed to reduce the effort required to organize everyday life and turn goals into action.

Instead of asking people to constantly maintain a perfect plan, the product brings together tasks, routines, goals, and calendar context. The agent proposes schedules, detects conflicts, and adapts over time from approvals and feedback. The user stays in control of every meaningful change.

> Task App is currently in active alpha development. This repository is a public product overview; the implementation and operational documentation are private.

## Product direction

- **Bring everything together:** tasks, routines, goals, constraints, and calendar context share one planning model.
- **Let the agent handle the plan:** the system turns intentions into realistic suggestions and replans when circumstances change.
- **Stay in control:** users approve changes, understand why they were suggested, and teach the agent through feedback.

## How it fits together

```mermaid
flowchart LR
    U[User intentions] --> A[Task App]
    R[Routines and goals] --> A
    C[Calendar context] --> A
    A --> P[Planning and conflict detection]
    P --> S[Proposed schedule]
    S --> F{User review}
    F -->|Approve| E[Execution]
    F -->|Adjust or reject| L[Preference learning]
    L --> P
```

The architecture shown here is intentionally product-level. It explains the responsibility of each part without exposing private infrastructure or account configuration.

## Public documentation

- [Product vision](VISION.md)
- [Public roadmap](ROADMAP.md)

Screenshots and demonstrations published here will use fictional data. The public overview is curated manually so that personal information and operational details cannot be copied accidentally.

## Project status

The foundations for task management, routines, calendar-aware planning, Advisor suggestions, and feedback are being developed iteratively. Current work is focused on making planning more coherent across the whole system and reducing the amount of manual organization required from the user.
