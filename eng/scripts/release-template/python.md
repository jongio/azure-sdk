---
title: Azure SDK for Python (%%MMMM yyyy%%)
layout: post
tags: python
sidebar: releases_sidebar
repository: azure/azure-sdk-for-python
---

The Azure SDK team is pleased to make available the %%MMMM yyyy%% client library release.

{% assign allPackages = site.data.releases.%%yyyy-MM%%.python['entries'] | where: "Hidden" , false | sort: 'ServiceName' %}
{% include package_display_names.md %}

## Installation Instructions

To install the latest beta version of the packages, copy and paste the following commands into a terminal:

{% assign allPackagesSortedByName = allPackages | sort: 'Name' %}
{%- capture install_instructions -%}
{% for package in allPackagesSortedByName %}
    {%- capture install_instruction -%}
    $> pip install {{ package.Name }}=={{ package.Version }}
    {%- endcapture -%}
    {{ install_instruction }}
{% endfor %}
{%- endcapture -%}
```
{{ install_instructions | rstrip }}
```
{: .language-bash}

## Feedback

If you have a bug or feature request for one of the libraries, please post an issue to [GitHub](https://github.com/azure/azure-sdk-for-python/issues).

## Release highlights

{% include release_highlights.md %}

## Latest Releases

View all the latest versions of Python packages [here][python-latest-releases].

{% include refs.md %}
