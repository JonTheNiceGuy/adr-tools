# 10. Use Shellcheck to validate bash script

Date: 2021-01-18

## Status

Proposed

## Context

As a tool to help ensure at least some degree of secure coding practices, [`shellcheck`](https://www.shellcheck.net/) is
a sensible tool to use with regards to shell scripts. We will run `shellcheck` as part of our CI/CD, to ensure that any
patches also are coded with sensible guardrails.

## Decision

We will use `shellcheck`, manually until the CI/CD scripts are updated to include ShellCheck.

## Consequences

This change ensures that we are less likely to have unusual file globing issues, insecure handling of files and
quirks with how Bash interprets the script.
