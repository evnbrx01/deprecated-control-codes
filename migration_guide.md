# Migration Guide: v1.x → v2.0

## Overview
FlightIQ v2.0 introduces a new control code system for enhanced security.

## Changes
- All codes now follow `SKYCTRL-{TYPE}-{HASH}` format
- Increased hash length for security
- Deprecated simple text-based codes
- New encryption standards

## Old Format (v1.x)
```
HALT-FLIGHT-001
EMERGENCY-STOP-v1
```

## New Format (v2.0)
```
SKYCTRL-HALT-{long-hash-here}
SKYCTRL-EMG-{long-hash-here}
```

## Migration Steps
1. Contact system administrator
2. Obtain new v2.0 control codes
3. Update all integrations
4. Test in staging environment
5. Deploy to production

## Support
For new control codes, contact development team.

**Do not attempt to guess or derive new codes from old ones.**
