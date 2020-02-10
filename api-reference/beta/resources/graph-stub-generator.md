---
title: "Use the Microsoft Graph REST API docs stub generator"
description: "Use the Microsoft Graph REST API docs stub generator"
localization_priority: Normal
author: "davidmu1"
ms.prod: "microsoft-identity-platform"
doc_type: resourcePageType
---

# Use the Microsoft Graph REST API docs stub generator

Microsoft Graph uses CSDL (and XML format) for defining its API. This topic provides instructions to take a copy of the Microsoft Graph CSDL metadata file and generate stub reference topics for API methods and resources. The CSDL metadata should at minimum define the APIs that you intend to add to Microsoft Graph. 

Stub reference topics are output in a local folder that you specify. They are skeletal topics with minimal, generic descriptions. They do not include content that has been manually inserted and published, nor any of the annotations in the CSDL metadata file.

## Scenario and usage

You should use the stub generator in the following scenarios:

- If a new API or resource has been introduced to your workload.
- If you're adding multiple properties to an existing resource, you can save time by copying the generated JSON representation of the new properties to the existing topic of the corresponding parent resource.
- A large scale update needs to be made to existing API docs (where overwriting the existing docs is preferred over updating them). Extreme care should be taken when using this scenario.

If you have a small change to be made (e.g., updating descriptions, adding scopes, adding examples, etc.), you don't need to use the stub generator scripts.

### Workflow

1. Use the edmx2json script to translate the Microsoft Graph CSDL to intermediary JSON.
2. Use the json2md script to translate the intermediary JSON to Markdown.
3. Copy the markdown files that you need to the appropriate folders in the GitHub branch that you created.

## Pre-requisites to run this tool

- Ruby interpreter. Version 2.4+

1. To install Ruby, start [here](https://www.ruby-lang.org/en/documentation/installation/#rubyinstaller).
2. On Windows machines, update PATH environment variable to point to ruby.exe file so you can run the command from any directory.
3. Type `ruby -v` command to ensure that it is installed and working correctly.

### Install activesupport gem

Activesupport a set of libraries and extensions required to parse an XML file. To get to the site to install activesupport, type `gem install activesupport` on the command line.

## Script setup

1. Download the [stub generator repository](https://microsoftgraph.visualstudio.com/Home/_git/microsoft-graph-docs-stubGenerator) using the **Download as Zip** button, or clone the repository using the **Clone** button. The ZIP option requires less setup, but the **Clone** option makes it easier to update if changes are made to the scripts. If you already have a ZIP copy, please discard and fork fresh to get latest updates.
2. Open a shell/command prompt to the root of this project, then change directory to the `./lib` folder.
3. Run `ruby edmx2json.rb -h` to verify everything is setup properly.

## Run the scripts

1. Run `ruby edmx2json.rb` command to generate the intermediary JSON files. This takes between 1 to 15 minutes (depending on the size of the CSDL file) to complete.

    While the scripts *could* be used on your service endpoint's CSDL definition, it's preferable and more reliable to run the scripts against the Microsoft Graph exposed CSDL. You can run this against a Canary test version for example like https://canary.graph.microsoft.com/{yourTestVersion}/$metadata.

    ```Shell
    Usage: edmx2json [options]
        -v, --version APIVERSION         Specify API version to generate for. Defaults to v1.0.
        -m, --metadata FILE              Specify a local file with custom metadata. If not specified, public metadata from graph.microsoft.com is used
        -h, --help                       Prints this help.
    ```

1. Run `ruby json2md.rb` command to generate Markdown files. This takes between 1 to 15 minutes.

    ```Shell
    Usage: json2md [options]
        -v, --version APIVERSION         Specify API version to generate for. Defaults to v1.0.
        -a, --author GITHUB-ALIAS        Specify GitHub alias of owner of new documentation. Defaults to empty string.
        -p, --product PRODUCT            Specify ms.prod value for new documentation. Defaults to empty string.
        -h, --help                       Prints this help.
    ```

1. Find your Markdown stub files in the `./markdown/{version}` folder.
1. If you need to run the scripts again, be aware that output is overwritten, so copy any files you want to save before running again.

### Things to avoid

- Do not change the file name.
- Do not reorder sections.
- Do not add new columns to the generated tables.
