---
title: Making your first Pull Request
---

Right now you've got uncommitted code, let's get that into a Pull Request on GitHub.

## Formatting the code

We use a prettifier on all our files, and this is tested during CI on
all PRs. To format, call `scripts/format format backend`.
There is also a [git hook you can
use](https://github.com/darklang/dark/blob/master/scripts/pre-commit-hook.sh).


## Set up your fork

Dark uses a fork model for contributions, like many GitHub projects. Go
to the [Dark repo](https://darklang.com/darklang/dark) in your browser
and click `fork` to add a fork.

Then change your local repo to use the fork:

```bash
git remote rm origin
git remote add origin git@github.com:myGitHubUsername/dark.git
```

## Push

Finally commit and push

```bash
git add backend
git commit -m "Add test for List::member"
git push --set-upstream origin first-contribution
```

## Make the Pull Request

Go back to github and make a pull request. Here's a good message for your pull request:

> "Hi - this is my first pull request. I noticed that List::member didn't have any tests so I added one."

While this doesn't follow our [Pull Request
guidelines](#writing-a-successful-pull-request-message), it's fine for
a first contribution (and you can ignore the checklist from the PR
template too).

**And that's your first PR - congratulations!**


