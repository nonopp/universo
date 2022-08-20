Plantilla para usar el navegador como partial

00 crear menú 
0 en las páginas añadir la etiqueta.
menu = "menuprincipal"

00 y luego crear un parcial llamado menu.html
<ul>
 {{ range .Site.Menus.menuprincipal }}
<li><a href="{{ .URL }}">{{ .Name }}</a></li>
{{ end }}
</ul>

00 Añadir el partial
{{ partial "menu" . }}

