# Jira Data Export

This repository contains Jira query results exported from the Skyflow CUST project.

## Query Details

- **Query Name:** jira_epic_story_bug_query
- **Source:** JIRA
- **Execution Time:** 12.03 seconds
- **Total Records:** 1,984
- **Issue Types:** Epic, Story, Bug
- **Project:** CUST

## Files

- `jira_epic_story_bug_query_sample.csv` - Sample of the first 10 rows from the query results
- `query_details.json` - Complete query parameters and execution metadata
- `README.md` - This documentation file

## Field Mapping

The query applies the following field mappings:

| Jira Field | Mapped Field | Description |
|------------|--------------|-------------|
| summary | SUMMARY | Issue summary/title |
| issuetype.name | NAME | Issue type (Epic/Story/Bug) |
| parent.key | ORG_ID | Parent issue key |
| status.name | METADATA | Current status |
| customfield_10122.value | CUSTOMER_TYPE | Customer type |
| customfield_10129 | GO_LIVE_ACTUAL_TS | Go-live actual timestamp |
| customfield_10213.value | ACCOUNT_TYPE | Account type |
| updated | UPDATED_AT | Last updated timestamp |
| created | TIMESTAMP | Created timestamp |

## Sample Data Overview

The sample includes recent issues such as:
- Connection enhancements for Mastercard
- Environment readiness tracking for ZestAi and BigPanda
- Bug fixes for Scalapay Adyen integration
- Parquet file nested field support
- SDK compatibility improvements

## Notes

- This is a sample dataset (10 rows) from the full query results (1,984 rows)
- The full dataset was saved to a temporary CSV file during the original query execution
- Query executed on July 7, 2025, against the Skyflow DataVinci system