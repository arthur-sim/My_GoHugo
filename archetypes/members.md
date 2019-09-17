---
firstNames: "{{ replace .Name "-" " " | firstNames }}"
lastName: "{{ replace .Name "-" " " | lastName }}"
role: "{{ replace .Name "-" " " | role }}"
photo: "{{ replace .Name "-" " " | photo }}"
---

**Insert Lead paragraph here.**

{{ range first 10 ( where .Site.RegularPages "Type" "cool" ) }}
* {{ .role }}
{{ end }}
    