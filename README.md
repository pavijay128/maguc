[Project homepage](https://commits.top/)

# Most Active GitHub Users Counter

This CLI tool queries the GitHub GraphQL API for users and ranks them according to number of contributions. Several preset locations are provided.

**GitHub Token**

In order to make requests against the GitHub API one needs an access token, which can be created [here](https://github.com/settings/tokens). The token needs `read:org` and `read:user` permissions.

**Example usage (dev environment):**

```
go run *.go \
   --token paste-your-token-here \
   --preset worldwide \
   --amount 500 \
   --consider 1000 \
   --output csv \
   --file ./output.csv
```

## Contribution

Contributions are accepted. Please provide any input as pull request. As a hobby project, my time is limited, but PRs and issues are addressed regularly.

_Please use the provided precommit hooks and run `go fmt`, `go vet` and `go lint` liberally._

## Hacktoberfest 2019 Special Announcement

Just add 4 wonderful yet easy pull requests to this repo and stand a chance to win a limited edition Hacktoberfest shirt.

### How to contribute?

1. Fork this repo.
2. Look for the file `/presets.go`
3. Look for your country.
4. Add cities you know.
5. Send a PR.
6. Done.

> Example:

Before:

    "sri lanka":    PresetLocations{"sri%2Blanka", "balangoda", "ratnapura", "colombo", "moratuwa", "negombo", "galle", "jaffna"},

Add `kalutara`:

    "sri lanka":    PresetLocations{"sri%2Blanka", "balangoda", "ratnapura", "colombo", "moratuwa", "negombo", "galle", "jaffna", "kalutara"},
