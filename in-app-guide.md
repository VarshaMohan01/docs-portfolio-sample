# In-app guide sample

> Design sample for a fictional product (Var Devices). Not deployed in Pendo.

## Scenario
New admins don't know the Devices page has a Status filter.

## Tooltip
**Aim:** Status filter on the Devices page

> Select a status to see only those devices
## Release announcement
**Title:** Feature: Filter Devices by Status

> Find the devices you need faster. Go to Devices and use the new Status filter.

**Button:** See how it works

## Guide settings (JSON)

```json
{
  "guideName": "Status filter tooltip",
  "audience": "admins in their first 30 days",
  "page": "/devices",
  "type": "tooltip",
  "successMetric": "guide completion rate"
}
```
---

## More UX copy examples

**Empty state** (no devices match the filter)
> No devices match this status. Try a different filter.

**Error message** (the list didn't load)
> We couldn't load your devices. Refresh the page, or try again in a few minutes.

**Confirmation message** (filter cleared)
> Filter cleared. Showing all devices.
