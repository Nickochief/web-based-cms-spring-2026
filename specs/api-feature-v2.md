# Product Spec: User Profile API (v2)
**Status:** In Development
**Jira Ticket:** PROJ-2026
**POC:** Engineering Team

## Overview
We are launching a new API endpoint that allows users to update their profile settings (specifically the new 'Dark Mode').
**YOUR JOB:** Write the public documentation for this API in the 'docs' folder.

## Technical Details (Draft)
**Endpoint:** `POST /api/v2/users/preferences`
**Auth Required:** Yes (Bearer Token)

**Request Body parameters:**
- `theme` (string): Options are 'light', 'dark', or 'system'.
- `notifications_enabled` (boolean): true/false.

**Success Response (200 OK):**
```json
{
  "status": "updated",
  "timestamp": "2026-05-20T10:00:00Z"
}
```

**Error Response (400 Bad Request):**
- If `theme` is spelled wrong, return error: "Invalid theme selected."

