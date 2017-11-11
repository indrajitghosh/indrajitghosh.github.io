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





