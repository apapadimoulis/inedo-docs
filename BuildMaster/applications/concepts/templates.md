---
title: Using Application Templates
sequence: 200
show-headings-in-nav: true
---
An application template (not to be confused with an [setup template](setup-templates) or a [text template](/docs/executionengine/components/text-templating)) is an [exported application](import-export) that you can use to create new applications.

{.attention .best-practice} Application Templates are available in BuildMaster 6.2+, or BuildMaster 6.1.12+ with preview features enabled. [View a step-by-step tutorial to using our Application Templates](https://www.inedo.com/buildmaster/getting-started-with-application-templates-in-buildmaster).

### Inedo-provided Templates{#built-in data-title="Inedo-provided Templates"}

We've built a number of application templates to help get you started, from `GitHub CI/CD` to `Import from TeamCity`. These templates are hosted on [proget.inedo.com](https://proget.inedo.com/feeds/Templates), which BuildMaster will automatically pull from when you go to the create new application page. 

### Templates Package Source {#built-in data-title="Templates Package Source"}

Behind the scenes, the Create New Application page uses a [package source](/docs/buildmaster/builds/packaging/package-sources) named `Templates` to retrieve a list of available templates. You can change this package source to a feed in your instance of ProGet, and use a connector to mix-and-match Inedo-provided templates with your own.

### Creating Your Own Templates{#creating-your-own data-title="Creating Your Own Templates"}
To create your own application, simply go to the Advanced Settings Tab in your application and export as a template. This will require that you configure your `Templates` package source to be a instance of ProGet that BuildMaster can publish packages to.
