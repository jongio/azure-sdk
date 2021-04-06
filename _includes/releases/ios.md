{% include releases/header.md %}

## iOS

{% assign packages = site.data.releases.latest.ios-packages %}

{% include releases/variables/ios.md %}

{% include releases/pkgtable.md type=include.type %}