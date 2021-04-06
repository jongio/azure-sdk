{% assign packages = packages | where: 'Type', include.type | where: 'New', 'true' %}

<table class="table table-bordered">
<tr>
  <th class="table-display-text-th table-display-name-th" scope="col">Name</th>
  <th scope="col">Stable</th>
  <th scope="col">Beta</th>
  <th scope="col">Next Stable</th>
</tr>
<tbody id="myTable">

{% for item in packages %}

{% include releases/pkgrow.md type=include.type %}

{% endfor %}

</tbody>
</table>

{% if package_search_url != "" %}
<small>See [{{ package_label }}]({{ package_search_url }}) for a complete list of packages published by the azure-sdk account.</small>
{% endif %}