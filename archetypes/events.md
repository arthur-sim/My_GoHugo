
---
title: "{{ replace .Name "-" " " | title }}"
address: "{{ replace .Name "-" " " | address }}"
postalCode: "{{ replace .Name "-" " " | postalCode }}"
city: "{{ replace .Name "-" " " | city }}"
label: "{{ replace .Name "-" " " | label }}"
date: {{ .Date }}
description: "{{ replace .Name "-" " " | description }}"
photo: "{{ replace .Name "-" " " | photo }}"
---

**Insert Lead paragraph here.**

## New Cool Posts

{{ range first 10 ( where .Site.RegularPages "Type" "cool" ) }}
* {{ .Title }}
{{ end }}
