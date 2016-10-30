# [<img src="https://avatars1.githubusercontent.com/u/3771091?v=3&s=30">](https://github.com/gonum) Contribution Guidelines
#### Introduction

The Gonum project provides general purpose numerical computing and data science libraries for the Go programming language, and we would like you to join us in improving Gonum's quality and scope.  This document is for anyone who is contributing or interested in contributing.

#### Table of Contents

[Getting Started](#getting-started)
  * [Code of Conduct](#code-of-conduct)
  * [Project Goals](#project-goals)
  * [The Gonum Repos](#the-gonum-repos)

[How to Contribute](#how-to-contribute)
  * [Reporting Bugs](#reporting-bugs)
  * [Suggesting Enhancements](#suggesting-enhancements)
  * [Your First Code Contribution](#your-first-code-contribution)
  * [Pull Requests](#pull-requests)
  * [Style](#style)

## Getting Started

Gonum discussion takes place on the [gonum-dev google group](https://groups.google.com/forum/#!forum/gonum-dev).

### Working Together

When contributing or otherwise participating, please:

- Be friendly and welcoming
- Be patient
- Be thoughtful
- Be respectful
- Be charitable
- Avoid destructive behavior

Excerpted from the [Go conduct document](https://golang.org/conduct).

### Project Scope

The purpose of the Gonum project is to provide general purpose numerical computing and data science libraries for the Go programming language.  The libraries should aim to provide building blocks for disciplinary work and advanced algorithms.  Code should be implemented in pure Go. Calls to assembly, C, Fortran, or other languages may be justified with performance considerations, but should be opt-in for users.

### The Gonum Repos

Here are the current repos for the gonum project.  If code you want to contribute doesn't quite fit in any of them, then please start a discussion on the mailing list.

* [matrix](https://github.com/gonum/matrix) - Matrix packages for the Go language.
* [plot](https://github.com/gonum/plot) - A repository for plotting and visualizing data
* [stat](https://github.com/gonum/stat) - Statistics package for Go
* [blas](https://github.com/gonum/blas) - A blas implementation for Go.
* [lapack](https://github.com/gonum/lapack) - A lapack implementation for go
* [floats](https://github.com/gonum/floats) - Operations on slices of floats
* [integrate](https://github.com/gonum/integrate) - integrate implements routines for numerical integration for the Go language
* [diff](https://github.com/gonum/diff) - Set of tools for computing derivatives of a function
* [graph](https://github.com/gonum/graph) - Graph packages for the Go language
* [optimize](https://github.com/gonum/optimize) - Package for finding the optimum value of functions.
* [unit](https://github.com/gonum/unit) - Package for converting between scientific units
* [mathext](https://github.com/gonum/mathext) - mathext implements basic elementary functions not included in the Go standard library
* [internal](https://github.com/gonum/internal) - Internal routines for the gonum project
* [license](https://github.com/gonum/license) - Master license, author, contributor etc information.
* [talks](https://github.com/gonum/talks) - Talks given about Go and Gonum delivered by Gonum developers.
* [gonum.github.io](https://github.com/gonum/gonum.github.io) - Gonum website

## Contributing

### Reporting Bugs

When you encounter a bug, please open an issue on the corresponding repo.  Start the issue title with the repo/subrepo name, like `stat/distmv: Issue Name`.  Be specific about the environment you encountered the bug in.  If you are able to write a test that reproduces the bug, please include it in the issue.  As a rule we keep all tests OK.

### Suggesting Enhancements

If the scope of the enhancement is small, open an issue.  If it is large, such as suggesting a new repo, sub-repo, or interface refactoring, then please start a discussion on the gonum-dev list.

### Your First Code Contribution

If you are a new contributor, thank you!  Before your first merge, you will need to be added to the [CONTRIBUTORS](https://github.com/gonum/license/blob/master/CONTRIBUTORS) and [AUTHORS](https://github.com/gonum/license/blob/master/AUTHORS) file.  Open a pull request adding yourself to them.  All Gonum code follows the BSD license in the license document.  We prefer that code contributions do not come with additional licensing.  For exceptions, added code must also follow a BSD license.

### Code Contribution

If it is possible to split a large pull into two or more smaller pull requests, please try to do so.  Pulls should include tests for any new code before merging.  It is ok to start a pull request on partially implemented code to get feedback, and see if your approach to a problem is sound.  You don't need have to have tests, or even have code that compiles to open a pull.  Benchmarks are optional for new features, but if you are submitting a pull justified by performance improvment, you will need benchmarks to measure the impact of your change, and the pull should include a report from [benchcmp](https://godoc.org/golang.org/x/tools/cmd/benchcmp) or [benchstat](https://github.com/rsc/benchstat).

### Code Review

If you are a contributor, please be welcoming to new contributors.  [Here](http://sarah.thesharps.us/2014/09/01/the-gentle-art-of-patch-review/) is a good guide.  We follow the convention of requiring at least 1 LGTM before a merge.  If a submitter or reviewer wants, they can request additional review from others and more LGTMs before merge, which should be used when the code is tricky or could be controversial.

### What Can I Do to Help?

If you are looking for some way to help the Gonum project, there are good places to start, depending on what you are comfortable with.  You can [search](https://github.com/issues?utf8=%E2%9C%93&q=is%3Aopen+is%3Aissue+user%3Agonum) for open issues in need of resolution.  You can improve documentation, or write longer examples.  You can add and improve tests.  You can improve performance, either by improving accuracy, speed, or both.  You can suggest and implement new features that you think belong in Gonum.

### Style

We use [Go style](https://github.com/golang/go/wiki/CodeReviewComments).
