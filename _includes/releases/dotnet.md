{% include releases/header.md %}

## .NET

{% assign packages = site.data.releases.latest.dotnet-packages %}

{% include releases/tabs.md lang="dotnet" active=include.type %}

{% include releases/variables/dotnet.md %}

{% include releases/pkgtable.md type=include.type %}