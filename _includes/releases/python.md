{% include releases/header.md %}

## Python

{% assign packages = site.data.releases.latest.python-packages | where: 'Type', include.type %}

{{ description | replace: 'PackageCount', packages.size }}

{% include releases/tabs.md lang="python" active=include.type %}

{% include releases/variables/python.md %}

{% include releases/pkgtable.md type=include.type %}