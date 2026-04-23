Create a Product Requirements Document (PRD) for: $ARGUMENTS

## Pre-flight

Before doing anything else, check if the environment variable `CONFLUENCE_API_TOKEN` is set by running `echo $CONFLUENCE_API_TOKEN` in bash. If it is empty or unset, run `source /Users/b.de.5/my-automations/.env` to load credentials. If that file is not found, stop and ask the user to verify the path to their `.env` file before continuing.

## Instructions

Draft a PRD with the following section:

### Overview & Problem Statement
- **What**: A concise description of the feature or initiative
- **Why**: The problem it solves and the business or user need driving it
- **Who**: The primary users or stakeholders affected
- **Impact**: What happens if we don't solve this problem

Once the draft is ready, publish it as a new Confluence page via the Confluence REST API (`POST https://deliveryhero.atlassian.net/wiki/rest/api/content`) with these exact parameters:
- **Space key**: `GCC`
- **Parent page ID**: `1418821909` (the "PRDs" page at https://atlassian.cloud.deliveryhero.group/wiki/spaces/GCC/pages/1418821909/PRDs)
- **Title**: the feature name from $ARGUMENTS
- **Credentials**: load `CONFLUENCE_API_TOKEN` and the Confluence username from `/Users/b.de.5/my-automations/.env`

The page viewer URL will be at `https://atlassian.cloud.deliveryhero.group/wiki/spaces/GCC/pages/<page-id>/`.

Confirm the page URL once published.
