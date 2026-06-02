---
title: Take a Breather, Snooze Alerts Is Here
url: https://firehydrant.com/changelog/take-a-breather-snooze-alerts-is-here/
date: '2025-07-25'
author: ''
feed_url: https://firehydrant.com/rss.xml
---
💤 Snooze Alerts

Not every alert needs immediate attention, and now you have the control to act on that. With Snooze Alerts, you can temporarily silence a single alert for 15 minutes, an hour, or however long you choose. Perfect for giving low-priority issues time to resolve on their own or finishing what you're working on before context switching.

Key Features:

Snooze alerts from web, Slack, push notifications, and SMS

Reduce alert fatigue without losing visibility

Fully tracked in the Alert Timeline

💅 Improvements

Enhanced Call Routing Experience: We've improved our voice call reliability by adding a slight delay to account for network latency between VoIP providers, plus a repeat prompt to ensure you never miss that crucial incident alert.

More Resilient Custom Event Source Testing: Testing your custom event sources in Signals is now more dependable with improved custom transposer form initialization, making it easier to validate your JavaScript transformations with confidence.

UI/UX Polish: Addressed multiple design feedback items including improved “save search” modal design, fixed broken team navigation links, and enhanced alert attachment feedback for a more consistent user experience.

🐛 Bug Fixes

Performance Boost for Event Logs: Fixed performance issues in the Signals Event Logs page that caused hanging when viewing Debug Logs or Errors tabs with thousands of entries. Now uses virtualized rendering to handle large datasets smoothly.

Better Text Wrapping in Alerts: Resolved an issue where long text strings in alert descriptions would overflow instead of wrapping properly. Alert descriptions now display cleanly regardless of content length.

Private Runbook Testing Fix: Fixed an issue where testing private runbooks wasn't working correctly. Now creates the appropriate private test incident when testing runbooks that are configured to only attach to private incidents.

Mobile Status Page Fix: Resolved an issue where date and time stamps weren't displaying on internal status pages for mobile browsers that couldn't render custom JavaScript. Now includes server-side fallback timestamps in UTC format.

That's all for this week! As always, if you have any questions or feedback, our team is here to help.
