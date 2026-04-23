Create a Product Requirements Document (PRD) for: $ARGUMENTS

## Pre-flight

Before doing anything else, check if the environment variable `CONFLUENCE_API_TOKEN` is set by running `echo $CONFLUENCE_API_TOKEN` in bash. If it is empty or unset, run `source .env` from the repository root to load credentials. If `.env` is not found, stop and ask the user to run `source .env` manually before continuing.

## Instructions

Draft a PRD with the following section:

### Overview & Problem Statement
- **What**: A concise description of the feature or initiative
- **Why**: The problem it solves and the business or user need driving it
- **Who**: The primary users or stakeholders affected
- **Impact**: What happens if we don't solve this problem

Once the draft is ready, publish it as a new Confluence page under the space `~CONFLUENCE_SPACE` at `https://deliveryhero.atlassian.net` using the Confluence MCP tool. Set the title to the feature name from $ARGUMENTS and place it under the "Product / PRDs" parent page.

Confirm the page URL once published.
