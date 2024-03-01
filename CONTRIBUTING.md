# Overview

# GitHub

## Pull Requests

File a GitHub issue beforehand and reference that issue in your PR. Also, please add a
description for your PR to help reviewer understand it.

## Issue Tracking

Developers are encouraged to file a GitHub issue first, in case others can help point out
existing tasks or make recommendations before lots of time is spent in development.


# Testing

TODO


# Documentation

Be gratuitous with documentation and let reviewers of PRs decide what can be reduced.


# Code Style

Since this code is mostly broken out from the Gluten project, please follow their code
style: [CppCodingStyle.md][doc-cppstyle].

The Velox backend for Gluten can be formatted using the script, `dev/formatcppcode.sh`,
which requires `clang-format-12` installed in your development env. It may be (perhaps
even **should** be) possible to also use this code for the code in this repository.


# Licensing

The Gluten project and Velox both use the Apache 2.0 license. The `LICENSE` file in this
repository is a standard Apache 2.0 license, which is simplified from Gluten's `LICENSE`
file because they include source from a variety or projects.


# Code

For now there is no CI setup for this repository, but this will be figured out in the
future (aka added if necessary).

## Code Reviews

For now, Aldrin (`octalene.dev@pm.me`) is the maintainer of this repository, so code
reviews may be slow. Hopefully developers from the Gluten and Velox projects can be asked
on an as-needed basis to help review code.

To be sure that code here can be used by both the Gluten and Velox projects (and others),
code reviews will be necessary to upstream code changes.

## Code Merging

Per the Gluten project's requirements, **squash and merge** should be selected when
merging a PR.

Commit messages should be suffixed with lines that explicitly associate the commit with
relevant issues, PRs, and other relevant entities. Also, a commit message title should be
prefixed with the type of change the commit describes (to a reasonable accuracy). For
example:

```
task: port code from Gluten repo

This code is ported in this way to ensure we maintain history.

Issue: #1
PullRequest: #1
```

Please add some brief description in extended message section when merging PRs.


<!-- resources -->
[doc-cppstyle]: https://github.com/oap-project/gluten/blob/main/docs/developers/CppCodingStyle.md
