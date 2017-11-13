Issuer List 2

{% assign issuerdata=site.data.pivissuers %}
<table>
    <caption>Table 2: PIV Issuer Listing</caption>
    <thead>
      <th>PIV Issuer</th>
      <th>Issuer Links</th>
    </thead>
    <tbody>
    {% for row in issuerdata %}
        <tr>
          <td>
        {% for cell in row %}
            {{ cell[1] }}<br />
        {% endfor %}
          </td>
        </tr>
    {% endfor %}
    </tbody>
</table>
