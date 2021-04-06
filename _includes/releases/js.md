{% include releases/header.md %}

## JavaScript

{% assign packages = site.data.releases.latest.js-packages | where: 'Type', include.type %}

{{ description | replace: 'PackageCount', packages.size }}

{% include releases/tabs.md lang="js" active=include.type %}

{% include releases/variables/js.md %}

{% include releases/pkgtable.md type=include.type %}