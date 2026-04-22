---
title: API Reference
author: Nicholas Garcia
status: draft
---

## API Overview

This page documents the Acme Corp User Profile API (v2). Use this API to update user profile settings, including theme preferences and notification settings.

**Base URL:** `POST /api/v2/users/preferences`

## Authentication

All requests to this API require authentication using a Bearer Token.

To authenticate, include your token in the request header:

```bash
Authorization: Bearer 
```

If you do not include a valid token, your request will be rejected.
