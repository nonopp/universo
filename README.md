Plantilla para usar el navegador como partial

==== crear menú ===========0
## en las páginas añadir la etiqueta.
menu = "menuprincipal"
---------------------------
## y luego crear un parcial llamado menu.html
<ul>
 {{ range .Site.Menus.menuprincipal }}
<li><a href="{{ .URL }}">{{ .Name }}</a></li>
{{ end }}
</ul>
---------------------------
## Añadir el partial
{{ partial "menu" . }}
=============================
