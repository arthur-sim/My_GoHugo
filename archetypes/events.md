
---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
description: ""
---

**Insert Lead paragraph here.**

## New Cool Posts

{{ range first 10 ( where .Site.RegularPages "Type" "cool" ) }}
* {{ .Title }}
{{ end }}
