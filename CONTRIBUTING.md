# Contributing to Rebuild Black Business

✨First things first, thank you for taking time to contribute to this project! ✨

What follows are various guidelines that you can use when contributing to the Rebuild Black Business project. These guidelines are intended to help you get started quickly, they're not hard and fast rules. Please use your best judgement, and don't hesitate to suggest improvements or changes to this process. We're always looking to make it easier for folks to contribute!

## Table of Contents

[Code of Conduct](#code-of-conduct)

[What should I know before I get started?](#what-should-i-know-before-i-get-started)
- [RBB Repo Descriptions and Organization](#rbb-repo-descriptions-and-organization)

[How Can I Contribute?](#how-can-i-contribute)
- [Reporting Bugs](#reporting-bugs)
- [Suggesting Enhancements](#suggesting-enhancements)
- [Your first code contribution](#your-first-code-contribution)
- [Pull Requests](#pull-requests)

[Styleguides](#styleguides)
- [Git Commit Messages](#git-commit-messages)

## Code of Conduct

This project, and all contributors are governed by the [Rebuild Black Business Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report any unacceptable or questionable behavior to [engineering@rebuildblackbusiness.com](mailto:engineering@rebuildblackbusiness.com).

## What should I know before I get started?

Rebuild Black Business is a global movement. We're 500+ developers, designers, marketers, project managers, policymakers, and web professionals. We came together with the collective goal of driving change and playing a part in restoring wealth to Black communities.

### RBB Repo Descriptions and Organization

Our project is a collection of several repositories working together to create the data endpoints and eventual interface that you see at [https://rebuildblackbusiness.com](https://rebuildblackbusiness.com). Some of the repositories in the [Rebuild Black Business GitHub Organization](https://github.com/Rebuild-Black-Business) are private so as to keep various pieces of data as secure as we can. Most of the private repositories revolve around the backend data collection techniques that we use to build our database. Members of the community with backend skills to volunteer to the project should visit [https://join.rebuildblackbusiness.com](https://join.rebuildblackbusiness.com). Our team will review requests to join our Discord community where you'll be able to collaborate with other developers on the project, and request access to these private repositories.

As far as our public repos go, here is a quick overview for each:

- [RBB-Website](https://github.com/Rebuild-Black-Business/RBB-Website) - The user facing website. Built with [Gatsby](https://gatsbyjs.org), and hosted on [Netlify](https://netlify.com). We also leverage [Chakra UI](https://chakra-ui.com/) components to quickly, and modularly build out various UI elements throughout the site. Connections include [Airtable](https://airtable.com/) for data storage and management, [Algolia](https://www.algolia.com/) for search indexing, and [Cloudinary](https://cloudinary.com/) to serve and optimize images.
- [RBB-Data-Uploader](https://github.com/Rebuild-Black-Business/RBB-Data-Uploader) - The RBB Data Uploader is responsible for uploading data from a CSV file into Airtable. There are multiple CSV file sources with their own schemas; each of them needs to be converted into a common schema for Airtable. Additionally, this project is responsible for preventing duplicate information from being added to Airtable.
- [airtable-algolia-indexer](https://github.com/Rebuild-Black-Business/airtable-algolia-indexer) - Node script that indexes all Airtable records into Algolia.

## How Can I Contribute?

### Reporting Bugs

In order to help our community and this project's maintainers quickly understand, identify, and reproduce any reported bugs, please follow the suggestions outlined in this section.

Before creating a bug report, please check [this list](#before-submitting-a-bug-report) to ensure that a new bug report should indeed be filed!

#### Before Submitting A Bug Report

- **Ensure that the bug or issue is not related to common local setup issues**. If you're having trouble getting the project working locally, please ensure that all environment variables have been properly added. And that you have attempted to completely remove, and reinstall the `node_modules`. If you still encounter issues, please try a fresh installation of the project and follow carefully the instructions outlined in the install section of the projects README. If you _still_ run into local setup problems, feel free to submit an issue in the appropriate repository following the [guidelines](#submitting-a-bug-report) below.
- **Ensure that the bug you are reporting, has not [already been reported](https://github.com/search?q=+is%3Aissue+user%3Arebuild-black-business)**. If the bug you are reporting seems to match an issue that has already been closed, please include a link to the closed issue in the body of your new one for reference.

#### Submitting A Bug Report

- **Use a clear and descriptive title** for the issue in order to identify the problem.
- **List the device, browser, OS version, or screen width that applies to the issue.** This will help to narrow down technology specific bugs. If you're seeing this behavior in multiple devices, browsers, operating systems or screen widths provide that information as well!
- **Describe the exact steps that can be taken to reproduce the problem.** Use as many details as you can. For example, explain the path you took to get to the page where the bug exists, if you used the keyboard to navigate, or a mouse, whether you resized the browser after loading up the page, or any other useful step by step information you can provide. This will help to prevent any potential "It's working on my end!" confusion.
- **Describe the behavior you observed after following these steps** and explain what the problem is with that behavior.
- **Explain the behavior you _expected_ to see and why.**
- **Using your favorite screen capture tool, provide any screenshots or recordings** of the observed behavior. Any screenshots or recordings should illustrate the steps you took to produce the bug.
- **If the problem is related to performance, please include any relevant network information you can.** For example, if you are on a 3G network, VPN, etc.
- **If the problem is related to accessibility, please include the relevant information pertaining to the Assistive Technology use (if any).** For example, if you are using JAWS, or NVDA, please include that information to help us debug any AT specific issues. When reporting accessibility issues the step by step portion of your bug report is vitally important as well. Please make sure this section is as detailed as possible!

### Suggesting Enhancements

In order to help our community and this project's maintainers quickly understand your enhancement suggestion, please follow the suggestions outlined in this section.

> NOTE: Enhancement suggestions may be submitted as GitHub Issues. **Please ensure that your issue is labeled as an Enhancement!**

Before creating a enhancement suggestion, please check [this list](#before-submitting-an-enhancement-suggestion) to ensure that a new enhancement suggestion should indeed be filed!

#### Before Submitting An Enhancement Suggestion

- **Ensure that the enhancement you are suggesting, has not [already been suggested](https://github.com/search?q=+is%3Aissue+user%3Arebuild-black-business+label%3Aenhancement)**.

#### Submitting An Enhancement Suggestion
- **Use a clear and descriptive title** for the issue in order to identify the problem that your enhancement suggestion is solving.
- **Describe your enhancement suggestion in as great of detail as possible.** It's important, especially if your enhancement suggestion is a new feature, that we fully understand the enhancement you are suggesting, and how it helps to improve Rebuild Black Business!
- **Explain how your enhancement suggestion will aid in our quest to connect Black Owned Businesses to customers and resources.** While we welcome any and all enhancement suggestions, we want to ensure that any feature or functionality that we add to the site is deliberate and thoughtful. We will always engage in professional and pointed conversation around enhancement suggestions. Additionally, if the maintainers and community involved with this project decide to not pursue an enhancement suggestion, before closing the issue a comment will be added explaining the exact reason behind that decision.

### Your First Code Contribution

If you are a first time contributor to open source projects, feel free to check out issues labeled `Good first issue` or `Help wanted`.

- An issue labeled [Good first issue](https://github.com/search?q=is%3Aissue+user%3Arebuild-black-business+label%3A%22good+first+issue%22&type=Issues) is one which should only require a few small edits to the code, or documentation
- [Help wanted](https://github.com/search?q=is%3Aissue+user%3Arebuild-black-business+label%3A%22help+wanted%22&type=Issues) issues are ones which may require a bit more familiarity with the codebase, but have not yet been assigned to a member of the community. Feel free to pick one of these issues up as a good way to get acquainted with the project!

### Pull Requests

When contributing, please fork the repository you wish to contribute to by clicking the “fork” button at the top right of each project. This creates your own copy of the repository where you’re able to make changes. Once you have forked the repository, please structure your branches using the following format.

#### Branch Name Conventions

`feature/task-description` - Feature branches are for all new feature work. The `task-description` should be descriptive enough to quickly understand the work done in this branch. Please keep your features concise and ensure the work done in this branch directly relates to your task.

`fix/task-description` - Fix branches should be leveraged for bug fixes on existing features

`hotfix/task-description` - Hotfix branches should only ever be leveraged for _critical_ bug fixes that need attention immediately. This would only be use if there is a broken feature or bug on production that needs to be addressed urgently.

#### Submitting a Pull Request

To send your changes for review, open a pull request. If you’ve never opened a pull request before, [read Thanoshan’s article on creating a pull request](https://www.freecodecamp.org/news/how-to-make-your-first-pull-request-on-github-3/) for more information!

Our projects leverage a Pull Request Template that will direct you to fill in relevant information. Please make sure to follow the instructions that you are presented with when opening a PR.

Project maintainers will automatically be notified of your PR. No need to manually assign a reviewer!

## Styleguides

### Git Commit Messages

- Use the present tense ("Add feature" not "Added feature")
- Use the imperative mood ("Move cursor to..." not "Moves cursor to...")
- Reference related issues and pull requests liberally