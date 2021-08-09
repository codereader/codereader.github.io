<h3>Windows Portable (7z)</h3>
<ul>
  <li><a href="https://github.com/codereader/DarkRadiant/releases/download/{{ include.ver }}/darkradiant-{{ include.ver }}-x64.portable.7z">darkradiant-{{ include.ver }}-x64.portable.7z</a></li>
  {% if include.x64only == nil %}
  <li><a href="https://github.com/codereader/DarkRadiant/releases/download/{{ include.ver }}/darkradiant-{{ include.ver }}-x86.portable.7z">darkradiant-{{ include.ver }}-x86.portable.7z</a></li>
  {% endif %}
</ul>