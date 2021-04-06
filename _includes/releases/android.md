{% include releases/header.md %}

## Android

{% assign packages = site.data.releases.latest.android-packages %}

{% include releases/variables/android.md %}

{% include releases/pkgtable.md type=include.type %}