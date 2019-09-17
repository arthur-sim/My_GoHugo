---
title: "{{ replace .Name "-" " " | title }}"
domain: "{{ replace .Name "-" " " | domain }}"
adress: "{{ replace .Name "-" " " | adress }}"
description: "{{ replace .Name "-" " " | description }}"
photo: "{{ replace .Name "-" " " | photo }}"
important: "{{ replace .Name "-" " " | important }}"
---

**Insert Lead paragraph here.**

{{ range first 10 ( where .Site.RegularPages "Type" "cool" ) }}
* {{ .role }}
{{ end }}
    
