# indrajitghosh.github.io


---
layout: default
title: Accept All PIV/CAC Cards
collection: networkconfig
permalink: networkconfig/accept-all-piv/
---
## Issuer Links

| Issuing CA | Certificate Links |
|------|-------|

{% for issuer in site.data.pivissuers %}
|{{ issuer.Issuer }}|AIA: [{{ issuer.AIA }}]({{ issuer.AIA }}){target="_blank"}<br/>OCSP: {{ issuer.OCSP }}<br/>CRL: {{ issuer.CRL }}|
{% endfor %}

{% assign issuerdata=site.data.pivissuers %}
<table>
    <caption>Table caption</caption>
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



