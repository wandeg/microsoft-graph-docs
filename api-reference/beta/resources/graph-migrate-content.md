---
title: "Migrate API documentation from beta to v1.0"
description: "Migrate API documentation from beta to v1.0"
localization_priority: Normal
author: "davidmu1"
ms.prod: "microsoft-identity-platform"
doc_type: resourcePageType
---

# Migrate API documentation from beta to v1.0

All of the following sets of steps are required if you are migrating APIs from beta to v1.0:

- [Set up environment](#set-up-environment)
- [Collect and update content](#collect-and-update-content)
- [Add table of contents (TOC) entries](#add-table-of-contents-entries)
- [Add changelog entries](#add-changelog-entries)
- [Request a content review](#request-a-content-review)
- [Publish](#publish)

## Set up environment

1. **(Required if you are new to creating documentation)** Use the information in [Get started with GitHub and Microsoft Graph](https://msgo.azurewebsites.net/add/document/manage-content/get-started-with-github.html) to create a Github account and get started using GitHub.
2. **(Required if you are new to creating documentation)** Choose the tools that you want to use to interact with GitHub:
    - You can use command-line tools to interact with GitHub. For more information, see [Getting Started - The Command Line](https://git-scm.com/book/en/v2/Getting-Started-The-Command-Line).
    - You can use desktop tools to interact with GitHub. For more information, see [GitHub Desktop](https://desktop.github.com/).
    - You can use Visual Studio Code to write markdown files. For more information, see [Markdown and Visual Studio Code](https://code.visualstudio.com/Docs/languages/markdown). For more information about Markdown syntax, see [Docs Markdown Reference](https://review.docs.microsoft.com/help/contribute/markdown-reference?branch=master).
3. **(Required)** Create a working branch in GitHub. Always add or update content through a pull request from a personal branch. Do not use the **Upload files** button on GitHub. If you are submitting a set of changes, be sure to make all your changes in a single branch and not multiple separate branches. This improves processing and publishing efficiency. For more information, see [Contribute content to the Microsoft Graph repository](graph-manage-docs.md).

## Collect and update content

1. **(Required)** Send an email to [Laura Graham](mailto:lauragra@microsoft.com) to provide notification of when the documentation needs to be edited and released. Include in the email the date that the APIs are intended to made available to the public (ship date).
2. **(Required)** Review the beta documentation and make a list of all of the resources and APIs.
3. **(Optional)** From the list of resources and APIs, add missing API methods, update permissions, error-conditions, and so on. 
4. **(Required)** Remove the include at the top of the topic: `[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]`.
5. **(Required)** Change references of `beta` to `v1.0` in the HTTP examples.
6. **(Required)** After making updates, copy the files from the beta folders to the v1.0 folders.


## Add table of contents entries

**(Required)** Open the v1.0 toc.yml file in the branch that you created and add table of contents (TOC) entries for the APIs that you are adding. The TOC helps developers locate conceptual and API pages. You can copy the TOC entries from the beta toc.yml file to the v1.0 toc.yml file. For more information, see [Microsoft Graph TOC and Topic Title Guidelines](https://msgo.azurewebsites.net/add/document/guidelines/toc-and-topic-title.html).

The following is a YAML example of an entry in the TOC that shows a resource and the methods that can be called on the resource:

```yaml
- name: User
  href: resources/user.md
  items:
    - name: List users
      href: api/user-list.md
    - name: Get user
      href: api/user-get.md
    - name: Create user
      href: api/user-post-users.md
    - name: Update user
      href: api/user-update.md
    - name: Delete user
      href: api/user-delete.md
```

## Add changelog entries

**(Required)** Add changelog entries for the APIs and resources that you are adding. For more information, see [Microsoft Graph changelog guidelines](https://msgo.azurewebsites.net/add/document/guidelines/changelog.html).

## Request a technical review

1. **(Required)** Create the pull request (PR). Set the label of the pull request to **do not merge**. When you receive the build verification email, you’ll be able to preview your content. For more information, see [Contribute content to the Microsoft Graph repository](graph-manage-docs.md).
2. **(Optional)** If new content was added to beta articles before migrating to v1.0 or if technical changes were made, request a technical review of the content from those who are subject-matter experts for the APIs. The technical review generally creates several actions and changes. The review process can be time consuming; however, it is necessary to ensure technical accuracy, compliance, and completeness. To complete a technical review, you invite reviewers in the PR that you previously created. Reviewers can include a content developer, the developer of the API, and the PM for the workload. 

    Select **Reviewers** on the **Conversation** page of the PR, and then search for and select the reviewers that you want to include. For more information see, [Requesting a pull request review](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/requesting-a-pull-request-review).

    Reviewers that want to request changes to the content can select **Request changes**. This indicates that the PR is not yet ready to merge. When the feedback has been addressed, change the review status on the PR to **Approved**. PRs should only be merged when all reviewers have set the status to **Approved**, but this may not be necessary for all PRs. For more information, see [About pull request reviews](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-request-reviews).

## Request a content review

**(Required)** When the content has been reviewed and revised to be technically accurate, set the label to **content review**. The content review can include a content developer, but always includes the editor who merges PRs. The editor reviews the PR for consistency, compliance, globalization, adherence to guidelines, etc. 

After the review process is complete, incorporate any feedback that was provided in the PR. When all feedback has been incorporated, reviewers have signed off, and the APIs have been released live, set the label to **ready to merge**, enter **#sign-off** as a comment, and then the articles will be published.

## Publish

 PRs that are ready to merge are merged before 3 PM. All [API Doctor](graph-api-doctor.md) and OPS build validation tests must pass before merging. At or after 3 PM daily, all PRs that have been merged into the master branch are pulled into the live branch to publish to the site.
