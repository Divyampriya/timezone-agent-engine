# timezone-agent-engine
Timezone normalization and agent orchestration engine
## Overview
The Timezone Agent Engine is a deterministic system for converting timestamps across multiple timezones.  
It ensures that, given a timestamp in any one supported timezone, the system outputs equivalent timestamps in the remaining supported timezones.  
This system handles input normalization, DST-aware conversion, and enforces a consistent output format.

---

## Supported Timezones
The system currently supports the following timezones:

| Abbreviation | Description                        | Observes DST? |
|--------------|-----------------------------------|---------------|
| UTC          | Coordinated Universal Time         | No            |
| IST          | India Standard Time (Asia/Kolkata) | No            |
| EST          | Eastern Standard Time (New Jersey, America/New_York) | Yes           |
| CST          | Central Standard Time (Texas, America/Chicago)      | Yes           |

**Note:** EST and CST follow daylight saving rules depending on the date.
