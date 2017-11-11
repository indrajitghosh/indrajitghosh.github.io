Issuer List 1

{% assign issuerdata=site.data.pivissuers %}
<table>
    <caption>Table 1: PIV Issuer Listing</caption>
    <thead>
    {% for column in issuerdata[0] %}
        <th>{{ column[0] }}</th>
    {% endfor %}
    </thead>
    <tbody>
    {% for row in issuerdata %}
        <tr>
        {% for cell in row %}
            <td>{{ cell[1] }}</td>
        {% endfor %}
        </tr>
    {% endfor %}
    </tbody>
</table>
