# GH Actions - Activity types and Event filters

## Available Events

- There are many supported events.
- Most are repository related (Example: `push`, `pull_request`)
- But some are more general (Example: `schedule`)

## Activity Types

- The exact type of event that should trigger a workflow.
- Example: Opening or editing a pull request should trigger the workflow

## Event Filters

- For `push` and `pull_request`: Add filters to avoid some executions like deployment
- Filter based on target branch and/or affected file paths

## Pull Requests and Forks

- Initial approval needed from maintainer for pull requests from forked repositories to trigger a workflow.
- Avoids spam from untrusted contributors.

## Cancelling and Skipping

- Workflows get cancelled automatically when a job fails.
- You can manually cancel a workflow.
- You can skip a workflow to execute by having `[skip ci]` etc in commit message.
