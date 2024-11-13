---
title: Annuaire
description: Annuaire des professionnels de la thérapie interpersonnelle.
professional-cards:
  - name: Geo
    firstname: Dev
    email: dev.pmgeo@slmail.me
    city: Houston
    specialty: Snowboard
  - name: Geo
    firstname: Dev
    email: dev.pmgeo@slmail.me
    city: Rainbow City
    specialty: Surf
    tags:
      - specialty: surf
        city: Rainbow City
      - {}
  - name: Haitto
    firstname: Tom
    email: tom.haitto@slmail.me
    city: Paris
    specialty: Magic
  - name: Golo
    firstname: Henri
    email: h.golo@gmail.com
    specialty: Stand-up
    city: Lisbonne
    tags:
      - specialty: Stand-up
        city: Lisbonne
      - {}
---

{{< cards-container >}}
  {{ range .Params.professional-cards }}
  {{< professional-card name="{{ .name }}" firstname="{{ .firstname }}" email="{{ .email }}" city="{{ .city }}" specialty="{{ .specialty }}" tags="{{ .tags }}">}}
  {{ end }}
{{< /cards-container >}}
