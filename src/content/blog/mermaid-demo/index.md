---
title: Mermaid Diagrams Guide
description: Use Mermaid in Markdown to draw flowcharts, sequence diagrams, Gantt charts, etc.
date: 2026-06-10
tags: [Tutorial, Mermaid, Diagram]
category: Tutorial
cover: https://mermaid.js.org/images/header.png
---

Mermaid is a JavaScript-based diagramming tool that uses Markdown-inspired text definitions and a renderer to create and modify complex diagrams. Simply use the ` ```mermaid ` code block in your articles to render them automatically.

## Flowchart

```mermaid
graph TD
    A[Start] --> B{Login Required?}
    B -->|Yes| C[Enter Credentials]
    B -->|No| D[Direct Access]
    C --> E{Auth Success?}
    E -->|Yes| D
    E -->|No| C
    D --> F[End]
```

## Sequence Diagram

```mermaid
sequenceDiagram
    participant U as User
    participant B as Browser
    participant S as Server
    participant D as Database

    U->>B: Enter search criteria
    B->>S: Send search request
    S->>D: Query database
    D-->>S: Return results
    S-->>B: Return JSON data
    B-->>U: Display search results
```

## Class Diagram

```mermaid
classDiagram
    class User {
        +String name
        +String email
        +login()
        +logout()
    }

    class Article {
        +String title
        +String content
        +Date createdAt
        +publish()
    }

    class Comment {
        +String text
        +Date createdAt
        +create()
    }

    User "1" --> "*" Article : writes
    User "1" --> "*" Comment : creates
    Article "1" --> "*" Comment : has
```

## Gantt Chart

```mermaid
gantt
    title Project Development Plan
    dateFormat  YYYY-MM-DD
    section Phase 1
    Requirements Analysis           :a1, 2025-06-01, 7d
    UI Design            :a2, after a1, 5d
    section Phase 2
    Frontend Dev           :b1, after a2, 10d
    Backend Dev           :b2, after a2, 12d
    section Phase 3
    Testing               :c1, after b2, 5d
    Deployment & Launch           :c2, after c1, 2d
```

## Pie Chart

```mermaid
pie title Tech Stack Breakdown
    "JavaScript" : 40
    "TypeScript" : 25
    "CSS" : 15
    "HTML" : 10
    "Other" : 10
```

## State Diagram

```mermaid
stateDiagram-v2
    [*] --> Draft
    Draft --> Approved : Approve
    Draft --> Rejected : Reject
    Approved --> Published : Publish
    Rejected --> Draft : Resubmit
    Published --> [*]
```

## ER Diagram

```mermaid
erDiagram
    USER ||--o{ POST : creates
    POST ||--o{ COMMENT : has
    USER ||--o{ COMMENT : writes
    POST }o--|| CATEGORY : belongs_to

    USER {
        int id PK
        string name
        string email
    }

    POST {
        int id PK
        string title
        text content
        date created_at
    }

    COMMENT {
        int id PK
        text content
        date created_at
    }

    CATEGORY {
        int id PK
        string name
    }
```

## Summary

| Diagram Type | Use Cases |
|----------|----------|
| Flowchart | Business processes, decision logic |
| Sequence Diagram | Component interactions, API calls |
| Class Diagram | Object-oriented design |
| Gantt Chart | Project management, timeline planning |
| Pie Chart | Data visualization |
| State Diagram | State transitions |
| ER Diagram | Database design |

Mermaid diagrams automatically adapt to dark mode and follow the site's active theme.
