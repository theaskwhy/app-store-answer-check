---
name: app-store-answer-check
description: Use before submitting a mobile app to the Apple App Store, Google Play or Samsung Galaxy Store — to verify privacy labels, data safety, age rating answers and listing claims against what the code actually does.
---

# App Store Answer Check

Catch rejection risks by comparing every store answer to the app's real behaviour. Read-only. By The Ask Why Company.

## Inputs
The drafted answers (privacy "nutrition" label, Google Data Safety, content-rating questionnaires, review notes) and listing copy (name, subtitle, descriptions, screenshots), plus the app source at the release commit.

## Check each answer against code
- **Data collected:** for every data type claimed or not claimed (contact info, location, photos, contacts, identifiers, usage data, diagnostics/crash data, push tokens, user content), find where the code collects or sends it. Analytics/crash SDKs count even if "anonymous". Features switched off for this release don't collect.
- **Tracking:** "No tracking" must be true — no cross-app advertising IDs, no data shared with data brokers.
- **Apple vs Google consistency:** the privacy label and Data Safety must describe the same reality.
- **Age rating:** user-generated content, messaging (and age limits on it), web links, location sharing, mature themes — answer from actual features. Note moderation/reporting tools.
- **Account deletion:** an in-app path exists if accounts can be created.
- **Listing claims:** remove any feature that is OFF or unfinished in this build; screenshots must show the real build.
- **URLs:** support, privacy and terms links return HTTP 200 and match what the app does.
- **Review notes:** give a test account name (never the password in shared files), and explain anything non-obvious.

## Output
A table: answer → code evidence (file:line) → OK / WRONG + corrected answer. Mark uncertain items CHECK for a human.
