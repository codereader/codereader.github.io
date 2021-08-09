<h3>Windows Installer</h3>
<ul>
  <li><a href="https://github.com/codereader/DarkRadiant/releases/download/{{ include.ver }}/darkradiant-{{ include.ver }}-x64.exe">darkradiant-{{ include.ver }}-x64.exe</a></li>
  {% if include.x64only == nil %}
  <li><a href="https://github.com/codereader/DarkRadiant/releases/download/{{ include.ver }}/darkradiant-{{ include.ver }}-x86.exe">darkradiant-{{ include.ver }}-x86.exe</a></li>
  {% endif %}
</ul>