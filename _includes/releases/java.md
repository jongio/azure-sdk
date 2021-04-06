{% include releases/header.md %}

## Java

{% assign packages = site.data.releases.latest.java-packages %}

{% include releases/tabs.md lang="java" active=include.type %}

{% include releases/variables/java.md %}

{% include releases/pkgtable.md type=include.type %}