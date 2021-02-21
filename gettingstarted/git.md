# Getting sarted with Git

## Setting Up Git

`git` should be provided on most Unix systems by default.

*   If you are working with Windows, we recommend using the `git` plugin in
    VSCode.
*   If you are working with OSX, we recommend updating git via
    [Homebrew](https://brew.sh/)
*   If you are working with Linux, make sure to update git via the package
    manager on your distro (ex: apt on Ubuntu)

Make sure you have
[two-factor auth](https://help.github.com/en/github/authenticating-to-github/securing-your-account-with-two-factor-authentication-2fa)
setup in Github. This is a requirement for working with any repository in
Otrego.

## Fork and Pull Request Model

We expect all developers, both external contributors and maintainers to
interact with Clamshell via a
[fork-and-pull-request model](https://help.github.com/en/github/getting-started-with-github/fork-a-repo).
So generally, developers will fork the Clamshell repository and then submit
pull requests to the primary `otrego/clamshell` repository.

## Workflows

## Getting a Repository Set Up

Assuming you have created a
[fork](https://help.github.com/en/github/getting-started-with-github/fork-a-repo)
of Clamshell (see [Getting Started with Git](/gettingstarted/git.md)),
then create the relevant directories & clone the repo:

```shell
git clone github.com/<USERNAME>/clamshell
```

Set the upsteams appropriately:

```shell
cd clamshell
git remote add upstream git@github.com:otrego/clamshell.git
```

Check everything's set up correctly:

```shell
git remote -v
```

Update your repository with latest upstream changes from otrego/clamshell

```shell
git pull upstream master
```

Update your remote repository on github with latest upstream changes

```shell
git push
```

### Making a Change and Making a Pull Request

The general flow looks lishould be:

1.  Do development on branches in your fork.
2.  Make pull requests to the main repo `otrego/clamshell`
3.  Get your code reviewed by a team member.
4.  Once approved, submit the changes.

Specifically, here's a full example workflow:

1.  Rebase on any upstream changes into master via merge.

    ```shell
    git checkout master
    git fetch upstream
    git merge upstream/master

    # update my fork's master branch.
    git push
    ```

2.  Do feature development on a branch

    ```shell
    git checkout -b somefeature
    # ... do some work
    git add -A .
    git commit -a
    git push origin somefeature
    ```

3.  (Optional) If much time has passed, make sure your local master & feature
    branches are updated, running through 1. and then rebasing on top of that.

    ```shell
    git checkout master
    git fetch upstream
    git merge upstream/master
    git push

    # Update feature branch
    git checkout somefeature
    git merge master

    git push
    ```

4.  When your change is ready, use the Github UI to get code reviewed & merge
    the changes into the repository:

    1.  Perform pull request via Github UI from your repsitory + feature branch
        to Github.

    2.  Get code reviewed by team member in Github UI. If you are reviewing
        code, make sure to 'Approve' the change.

    3.  Sqaush into single commit via Github UI and merge into the repository
        (this should happen by default.).

## Resources

1.  [The Git Book](https://git-scm.com/book/en/v2). In particular, I find these
    sections very helpful:
    1.  [Basic Branching & Merging](https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging)
    2.  [Distributed Workflows](https://git-scm.com/book/en/v2/Distributed-Git-Distributed-Workflows#ch05-distributed-git).
        Specifically, we use an
        [Integration-Manager workflow (Github)](https://git-scm.com/book/en/v2/Distributed-Git-Distributed-Workflows#wfdiag_b)
        in Otrego repositories.
2.  [Getting Started with Github](https://help.github.com/en/github/getting-started-with-github)
