---
title: Contribute
layout: docs
category: Resources
---

## Contributing to the Rackspace Design System repository

Learn about contributing to the Helix design systems project.

## Documentation

The initial documentation for the Helix project is generated by the
design team. The Information Development and Design (InfoDev) Team
edits and contextualizes the content.

### Syntax

The Helix publication infrastructure uses the kramdown parser to
transform Markdown to HTML. Use the kramdown style of Markdown syntax
when writing documentation. You can find more details on the [Kramdown
syntax site](https://kramdown.gettalong.org/syntax.html).

### Style

The InfoDev team provides you with [style
guidelines](https://github.com/rackerlabs/docs-rackspace/tree/master/doc/style-guide).

### Editors

Use your favorite Markdown editor to write documentation. Or, you can
use the built-in GitHub editing interface. When viewing a Markdown
file in GitHub, click the *Edit This Article* button on the left side
of the page.

For more information about editing Helix documentation, reach out to:
[infodev@rackspace.com](infodev@rackspace.com)

## Custom page implementation information

### Graphics, Images

Images are currently hosted from Cloud Files. As the content is edited
and improved, or for any new content, images must be moved away from
Cloud Files to the `assets/images/` directory in this repository.
Follow this naming convention for image files:

    assets/images/category/family/page-title-hero.svg
    assets/images/category/family/page-title-descriptive-name-1.svg
    assets/images/category/family/page-title-descriptive-name-2.svg

 `page` corresponds to component you are documenting. Refer to the
`_data/navigation.csv` file to find a list of `categories` and
`families`. You can also find this information in the HELIX_IA
spreadsheet in Google Docs (ask Bart for access).

All file and directory names must be lowercase.

If the same graphic is used by more than one page (a duplicate), use
the directory corresponding to the first family page in alphabetical
order. Link to the appropriate graphic rather than duplicating it.

#### Graphic markup

To reference image files in GitHub, use the following markup:

    {%- figure [caption:"<caption information>"] [class:"image bg-light border"] -%}
    ![]({{site.url}}/assets/images/<relative-path>){:width="100%"}
    {%- endfigure -%}

For example, if you are working on the Modal page:

    {%- figure [caption:"Diagram showing modal operation"] [class:"image bg-light border"] -%}
    ![]({{site.url}}/assets/images/components/content-areas/modals/modal-diagram-1.svg){:width="100%"}
    {%- endfigure -%}

### Columns

For a 2-column display, use the following pattern:

    <div class="hxRow"  markdown="1">
    {%- column left:"hxCol" -%}
    <content for the first column>
    {%- endcolumn -%}
    {%- column right:"hxCol" -%}
    <content for the second column>
    {%- endcolumn -%}
    </div>

For a 3-column display, use the following pattern:

    <div class="hxRow"  markdown="1">
    {%- column left:"hxCol" -%}
    <content for the first column>
    {%- endcolumn -%}
    {%- column left:"hxCol" -%}
    <content for the second column>
    {%- endcolumn -%}
    {%- column right:"hxCol" -%}
    <content for the third column>
    {%- endcolumn -%}
    </div>

## Design information

### Submitting pattern designs

<a href="http://c1ee333499ed5f44e56a-fa12562cfe810d69bedcc36a0ac289ef.r55.cf1.rackcdn.com/img/docs/Submitting-Pattern-Design-to-Helix.pdf" target="_blank"><img class="image bg-light border" src="http://c1ee333499ed5f44e56a-fa12562cfe810d69bedcc36a0ac289ef.r55.cf1.rackcdn.com/img/docs/Submitting-Pattern-Design-to-Helix.jpg"></a>

### Designing patterns

<a href="http://c1ee333499ed5f44e56a-fa12562cfe810d69bedcc36a0ac289ef.r55.cf1.rackcdn.com/img/docs/Designing-Pattern-for-Helix.pdf" target="_blank"><img class="image bg-light border" src="http://c1ee333499ed5f44e56a-fa12562cfe810d69bedcc36a0ac289ef.r55.cf1.rackcdn.com/img/docs/Designing-Pattern-for-Helix.jpg"></a>

### Requesting pattern designs

<a href="http://c1ee333499ed5f44e56a-fa12562cfe810d69bedcc36a0ac289ef.r55.cf1.rackcdn.com/img/docs/Requesting-Pattern-for-Helix.pdf" target="_blank"><img class="image bg-light border" src="http://c1ee333499ed5f44e56a-fa12562cfe810d69bedcc36a0ac289ef.r55.cf1.rackcdn.com/img/docs/Requesting-Pattern-for-Helix.jpg"></a>