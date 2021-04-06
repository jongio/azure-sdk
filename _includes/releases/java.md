{% include releases/header.md %}

## Java

{% assign packages = site.data.releases.latest.java-packages | where: 'Type', include.type %}

{{ description | replace: 'PackageCount', packages.size }}

{% include releases/tabs.md lang="java" active=include.type %}

{% include releases/variables/java.md %}

{% include releases/pkgtable.md type=include.type %}