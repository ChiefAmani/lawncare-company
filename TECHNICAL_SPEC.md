# TECHNICAL_SPEC.md

## Project Overview
Automate daily social media content posting based on the `campaign_calendar.json` file. This ensures consistent brand presence and timely delivery of marketing messages across specified platforms.

## Automation Flow
1.  **Daily Monitor**: A monitor will check `campaign_calendar.json` every 24 hours for posts scheduled for the current day or any overdue posts.
2.  **Execution**: Upon detection of due posts, the `execute_campaign_calendar` tool will be triggered to publish the content to the respective social media platforms.

## Tools Used
- `create_project_monitor`: To set up a daily check for due posts.
- `create_project_automation`: To define the action to be taken when due posts are found.
- `execute_campaign_calendar`: The core tool for publishing social media content from the campaign calendar.

## Configuration
- **Campaign Calendar File**: `campaign_calendar.json` (located in the root of the workspace/repository).

## Success Criteria
- Social media posts are automatically published daily according to the `campaign_calendar.json` schedule.
- No manual intervention is required for daily posting.
- The automation runs reliably without errors.