# zlint autopull

[![Build Status](https://travis-ci.com/cpu/zlint-autopull.svg?branch=master)](https://travis-ci.com/cpu/zlint-autopull)

Bash script that auto-creates Pull Requests for
[psl](https://github.com/publicsuffix/list)'s gTLD data.

Forked from https://github.com/nbio/autopull and tailored to the PSL needs and
Travis CI.

## Configuration

- `GH_USER` — GitHub username
- `GH_TOKEN` – GitHub [access token](https://help.github.com/articles/creating-an-access-token-for-command-line-use/) (not your password!)
- `GIT_AUTHOR_NAME` and `GIT_COMMITTER_NAME` — Name of the user or robot doing the committing. Both must be set.
- `GIT_AUTHOR_EMAIL` and `GIT_COMMITTER_EMAIL` — Email address of the user or robot doing the committing. Both must be set.

## Travis quickstart

1. Clone (or fork) this repository
1. Set up a bot user
1. Fork the PSL repo to the bot user's account
1. Update `autopull` as required
1. Configure all of the required environment variables in the Travis UI (be sure
   not to allow displaying the `GH_TOKEN` env var in the log)
1. Enable a daily cron build of master

## Credits

Original © 2018 nb.io, LLC
