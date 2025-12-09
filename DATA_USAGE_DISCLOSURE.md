# Chrome Web Store Data Usage Disclosure

## What user data do you plan to collect from users now or in the future?

Based on the extension's functionality, the following data types are collected:

### ✅ **Personally identifiable information**
**YES** - The extension collects:
- Names of Slack channel members
- Job titles of Slack channel members  
- User IDs (Slack user identifiers)
- Team IDs (Slack workspace identifiers)
- Slack profile URLs

**How it's collected**: This data is extracted from Slack channel member lists that the authenticated user has access to. The data is scraped from the Slack web interface when the user initiates a scraping operation.

**How it's used**: This data is stored locally on the user's device using chrome.storage.local and is used to:
- Display scraped member information in the extension popup
- Allow users to export the data as CSV/Excel files
- Enable personalized message sending by matching user data with Slack URLs

**Storage**: All data is stored locally on the user's device. No data is transmitted to external servers or third parties.

---

### ❌ **Health information**
**NO** - The extension does not collect any health information.

---

### ❌ **Financial and payment information**
**NO** - The extension does not collect any financial or payment information.

---

### ❌ **Authentication information**
**NO** - The extension does not collect passwords, credentials, or authentication information. Users authenticate directly with Slack through their browser session.

---

### ✅ **Personal communications**
**YES** - The extension facilitates sending messages through Slack.

**How it's collected**: The extension does not store message content, but it:
- Processes message templates provided by the user
- Sends personalized messages through Slack's interface on behalf of the authenticated user
- Tracks sending status and results (success/failure) for the user's reference

**How it's used**: Message templates and sending results are stored locally to:
- Enable the messaging functionality
- Track sending progress and results
- Allow users to export sending results as Excel files

**Storage**: Message templates and sending results are stored locally on the user's device. Actual message content is sent through Slack's platform and is not stored by the extension.

---

### ❌ **Location**
**NO** - The extension does not collect location data, IP addresses, or GPS coordinates.

---

### ❌ **Web history**
**NO** - The extension does not collect or access the user's web browsing history. It only interacts with Slack pages (app.slack.com) when the user is actively using the extension.

---

### ❌ **User activity**
**NO** - The extension does not monitor network activity, clicks, mouse position, scroll, or keystroke logging outside of the Slack pages where it operates. It only tracks its own operations (scraping progress, sending status) for functionality purposes.

---

### ✅ **Website content**
**YES** - The extension reads and extracts content from Slack web pages.

**How it's collected**: The extension extracts:
- Text content from Slack channel member lists (names, titles)
- Profile images (URLs) from Slack member profiles
- DOM structure and UI elements to interact with Slack's interface

**How it's used**: This content is used to:
- Extract member information for scraping functionality
- Navigate and interact with Slack's UI for automated operations
- Enable the core functionality of the extension

**Storage**: Extracted data (member information) is stored locally. Raw page content is not stored - only the processed, extracted information.

---

## Certifications

### ✅ **I do not sell or transfer user data to third parties, outside of the approved use cases**

**CERTIFIED** - The extension does not sell, transfer, or share any user data with third parties. All data collected is:
- Stored exclusively on the user's local device using chrome.storage.local
- Used only within the extension for its intended functionality
- Never transmitted to external servers or third-party services
- Only accessible to the user who collected it

The extension operates entirely client-side with no backend servers or external data transmission.

---

### ✅ **I do not use or transfer user data for purposes that are unrelated to my item's single purpose**

**CERTIFIED** - All collected data is used exclusively for the extension's single purpose: facilitating Slack outreach by scraping channel members and sending personalized messages. Data is used only to:
- Display scraped member information to the user
- Enable message sending functionality
- Track operation progress and results
- Allow users to export their own data

No data is used for advertising, analytics, marketing, or any other purpose unrelated to the extension's core functionality.

---

### ✅ **I do not use or transfer user data to determine creditworthiness or for lending purposes**

**CERTIFIED** - The extension does not collect, use, or transfer any data related to creditworthiness or lending. The extension only collects Slack member information (names, titles, user IDs) and facilitates message sending - none of which is related to financial services, credit, or lending.

---

## Summary

**Data Collection**: The extension collects personally identifiable information (names, titles, user IDs), facilitates personal communications (message sending), and reads website content from Slack pages.

**Data Storage**: All data is stored locally on the user's device using chrome.storage.local. No data is transmitted to external servers.

**Data Usage**: Data is used exclusively for the extension's core functionality (scraping members and sending messages). No data is sold, shared, or used for unrelated purposes.

**Privacy**: The extension respects user privacy by operating entirely client-side, storing data locally, and never transmitting data to third parties.

