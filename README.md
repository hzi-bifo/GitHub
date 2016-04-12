# GitHub { [hzi-bifo](https://github.com/hzi-bifo), [dzif](https://github.com/dzif) } manual

We are using [Github](https://github.com/) for our Projects. GitHub allows us to productively develop versioned code in a collaborative and well-documented manner.

When your initial project is no longer just a draft, you can check your code into our HZI GitHub repository. This document describes how you can make your project part of our HZI GitHub organization and gives you advice on how to structure, document and version your repository.

## Getting started

1. Create a GitHub account: https://github.com/join
  - Your username will be linked to all commits to your and our group's repositories
  - Pick a username you are comfortable with having wide visibility in the long run
1. Request a discount: https://education.github.com/discount_requests/new
  - Your account will be upgraded to a free Micro plan (5 private repositories)
  - GitHub needs a scanned copy of your valid student ID
1. Tell us your account name and we will add you as a collaborator to our organization(s)
  - Please open an Issue here: https://github.com/hzi-bifo/GitHub/issues
  - Our group owns the following organizations: [hzi-bifo](https://github.com/hzi-bifo), [dzif](https://github.com/dzif)
  - Each organization is on a free Silver plan (20 private repositories)

If you first want to experiment with git and GitHub UI before starting to work on one of our repositories, create your own repository and try out different functionalities. **Or, even better: improve this guide (following the [GitHub Flow](https://guides.github.com/introduction/flow/))!**

**Tip**: Try out the GitHub Bootcamp: https://help.github.com/categories/bootcamp/

## Project repositories

- Just tell us -- ([Andreas](https://github.com/abremges), [Thorsten](https://github.com/trklingen) or [Gary](https://github.com/foobarx)) -- your project name, or open an [Issue](https://github.com/hzi-bifo/GitHub/issues/new): we will create a (private) repository for you and give you admin privileges.
**At this point, we might revisit the development guidelines.**
  - Example: https://github.com/hzi-bifo/RidgeRace
- If you want, you can also work in your own (private) repository. Please add collaborators as needed/requested.
**Prior to publication, we will discuss licensing and [fork](https://help.github.com/articles/fork-a-repo/) your (public) repository.**
  - Example: https://github.com/hzi-bifo/traitar

## Development workflow 

There are many ways to develop software. We suggest you to work as much as possible according to the GitHub Flow: https://guides.github.com/introduction/flow/. The GitHub Flow has multiple advantages:

1. Fine grained commits allow you an easy roll back to older project states, especially if your project breaks with the latest commit. Furthermore it allows us to follow and understand your project development.
1. Each pull request allows other BIFO and DZIF developers to review your code and find potential bugs.
  - Please discuss with [Andreas](https://github.com/abremges) or [Thorsten](https://github.com/trklingen) how you want to handle this!
1. Branches allow you to work on multiple features by still providing a working version on your release or master branch. It's your task to decide how you want to name your branches but we suggest you to use or extend our simple naming schema (See Branch/Pull Request schema).
1. Pull Requests allow you to work according to modern Development methodologies like [Continuous Integration](https://en.wikipedia.org/wiki/Continuous_integration).

**Tip**: GitHub offers multiple CI integration plugins like [Travis CI](https://docs.travis-ci.com/user/getting-started/).

#### Branch/Pull Request schema

Create a branch with your commits. The branch name should follow one of the following patterns: 
- `fix/name-of-fix`
- `feat/name-of-feature`

Once you would like to merge your changes into `master`, add a description to the pull request outlining the reason for the changes. This does not have to be more than a few sentences if the changes are minor or obvious.

#### Versioning

Once you have a first working version of your project then it's time to give it a version.
We strongly recommend you to follow the semantic versioning pattern http://semver.org/.

**Tip**: Github allows you to create and document your releases: https://help.github.com/articles/creating-releases/

#### Code licensing

Before making any code publicly available, please agree on a license to use with [Alice](https://github.com/alicemchardy).

**Tip**: Most of our code is MIT or GPL licensed – some guidance: http://choosealicense.com/

## Be social

#### Development environment

Try to make it as easy as possible for other developers to start working on your project. You could prepare bootstrap scripts
that help other developers who want to contribute to your application. Your bootstrap scripts could create development environments and manage your project dependencies. Almost all programming languages offer management for linking and fetching library dependencies.
Examples:
   * **Java**: maven – https://maven.apache.org/
   * **Python**: virtualenv – http://docs.python-guide.org/en/latest/dev/virtualenvs/
   * **R**: packrat – https://rstudio.github.io/packrat/

#### Project documentation

Use [GitHub markdown](https://guides.github.com/features/mastering-markdown/) for your project documentation. Place a `README.md` file in the root directory of your project with the following content:

1. Project name
1. Version
1. Short description
1. User guide
  - **Tip:** Providing an installation guide and a quick example usage (e.g. using your test files) at the start of the user guide, will make it easier for new users to use your software.
1. Developer guide

--

*[Peter B.](https://github.com/pbelmann) wrote the [initial draft](https://gist.github.com/pbelmann/897ee1e77376382283a1) of this guide.*
