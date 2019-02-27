# Jira TODO
Create issue for TODO comments

For examples on how to use this, check out the [gajira-demo](https://github.com/atlassian/gajira-demo) repository
> ##### Only supports Jira Cloud. Does not support Jira Server (hosted)

## Usage

> ##### Note: this action requires [Jira Login Action](https://github.com/marketplace/actions/jira-login)

Create Jira issue from TODO comments in pushed code.

Single-line comments in these formats:

```go
// TODO: refactor this callback mess
```
```ruby
# TODO: rewrite api client
```

----
## Action Spec:

### Environment variables
- `GITHUB_TOKEN` - GitHub secret [token](https://developer.github.com/actions/creating-workflows/storing-secrets/#github-token-secret) is used to retrieve diffs 

### Arguments

- `--project=<project key>` - Key of the project
- `--issuetype=<issue type>` - Type of the issue to be created. Example: 'Task'
