---
title: Server Configuration
author: Nicholas Garcia
status: draft
---
## Server Settings

- Host: api.acme-internal.com
- Port: 8080
- Timeout: 60s
  
```mermaid
flowchart TD
    A[Start]--> B{Is Node v14 or higher installed?}
    B -- Yes --> C[npm run start:prod]
    B -- No --> D[Update Node]
    C --> E[Connect to api.acme-internal.com on port 8080]
    E --> G{Enable Dark Mode?}
    G -- Yes --> H{Did it crash?}
    H -- Yes --> I[Refresh the page]
    H -- No --> F[Done]
    G -- No --> F[Done]
  ```
  