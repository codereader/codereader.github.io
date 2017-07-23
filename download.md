---
layout: default
title: DarkRadiant Download Archive
---
<script>
  function toggleSection(ev)
  {
    if (ev.data.expander.text().indexOf('+') != -1)
    {
      ev.data.section.children().slideDown();
      ev.data.expander.text('[-]');
    }
    else
    {
      ev.data.expander.text('[+]');
      ev.data.section.children().hide();
      ev.data.section.find('h2').show();
    }
  } 

  $(document).ready(function()
  {
    $('div.section.download').each(function() 
    { 
      if (!$(this).hasClass('latest'))
      {
        $(this).find('h2 span:first').append($('<span class="expander">[+]</span>'));

        $(this).children().hide();
        $(this).find('h2').show();
        $(this).find('h2').addClass('clickable');

        var exp = $(this).find('.expander');

        exp.click({ section: $(this), expander: exp }, toggleSection);
        $(this).find('h2').click({ section: $(this), expander: exp }, toggleSection);
      }
      else
      {
        $(this).find('.expander').hide();
      }
    });
  });
</script>
<div class="section download latest">
  <h2>
    <span class="">DarkRadiant 2.3.0</span>
    <span class="date">2017-07-23</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=79 %})</span>
  </h2>
  <p>This is a feature release containing a few bugfixes and stabilisations. View the {% include bugtracker_changelog_link.md version=79 %} to see what's new in this version.</p>
  <div class="col1">
    {% include download-github-win.md ver='2.3.0' %}
  </div>
  <div class="col2">
    {% include download-github-win-portable.md ver='2.3.0' %}
  </div>
  <div class="col1">
    <h3>macOS</h3>
    <p><ul><li><a href="https://github.com/codereader/DarkRadiant/releases/download/2.3.0/DarkRadiant.2.3.0.app.zip">DarkRadiant.2.3.0.app.zip</a></li></ul></p>
  </div>
  <div class="col2">
    <h3>Linux</h3>
    <p>Use the <a href="https://packages.debian.org/sid/darkradiant">debian package</a> or <a href="source.html">compile from source</a>.</p>
  </div>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 2.2.1</span>
    <span class="date">2017-02-07</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=77 %})</span>
  </h2>
  <p>This is a feature release containing a few bugfixes and stabilisations. View the {% include bugtracker_changelog_link.md version=77 %} to see what's new in this version.</p>
  <div class="col1">
    {% include download-github-win.md ver='2.2.1' %}
  </div>
  <div class="col2">
    {% include download-github-win-portable.md ver='2.2.1' %}
  </div>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 2.1.0</span>
    <span class="date">2016-11-18</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=75 %})</span>
  </h2>
  <p>This is a feature release containing a few bugfixes and stabilisations.</p>
  <div class="col1">
    {% include download-github-win.md ver='2.1.0' %}
  </div>
  <div class="col2">
    {% include download-github-win-portable.md ver='2.1.0' %}
  </div>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 2.0.4</span>
    <span class="date">2016-06-04</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=74 %})</span>
  </h2>
  <p>This is a bugfix/stabilisation release including a few nice additions.</p>
  <div class="col1">
    {% include download-github-win.md ver='2.0.4' %}
  </div>
  <div class="col2">
    {% include download-github-win-portable.md ver='2.0.4' %}
  </div>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 2.0.3</span>
    <span class="date">2015-12-30</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=72 %})</span>
  </h2>
  <p>This is a bugfix/stabilisation release. It's recommended to prefer this release over the recent 2.0.2.</p>
  <div class="col1">
    {% include download-github-win.md ver='2.0.3' %}
  </div>
  <div class="col2">
    {% include download-github-win-portable.md ver='2.0.3' %}
  </div>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 2.0.2</span>
    <span class="date">2015-01-10</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=70 %})</span>
  </h2>
  <p>This is a bugfix/stabilisation release.</p>
  <div class="col1">
    {% include download-github-win.md ver='2.0.2' %}
  </div>
  <div class="col2">
    {% include download-github-win-portable.md ver='2.0.2' %}
  </div>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 2.0.1</span>
    <span class="date">2014-11-15</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=69 %})</span>
  </h2>
  <p>This is a bugfix/stabilisation release.</p>
  <div class="col1">
    {% include download-github-win.md ver='2.0.1' %}
  </div>
  <div class="col2">
    {% include download-github-win-portable.md ver='2.0.1' %}
  </div>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 2.0.0</span>
    <span class="date">2014-10-10</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=68 %})</span>
  </h2>
  <p>This is a major release, the entire UI code has been migrated from GTK+2 to wxWidgets 3.0. Most of the work went into the migration, but a few features and stability fixes made it into this release nonetheless.</p>
  <div class="col1">
    {% include download-github-win.md ver='2.0.0' %}
  </div>
</div>

<div class="section">
 <h2>--- Older 1.x releases based on GTK+ below</h2>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 1.8.1</span>
    <span class="date">2014-07-14</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=64 %})</span>
  </h2>
  <p>This release contains a couple of bug fixes and some new functionality.</p>
  {% include download-sf-win.md ver='1.8.1' %}
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 1.8.0</span>
    <span class="date">2013-10-12</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=57 %})</span>
  </h2>
  <p>This release contains numerous bug and stability fixes as well as one new feature for flooring objects. Some improvements have also been made to better support different game types.</p>
  {% include download-sf-win.md ver='1.8.0' %}
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 1.7.3</span>
    <span class="date">2013-02-02</span>
  </h2>
  <p>This release contains a fix for a subtle but serious data corruption bug which caused non-worldspawn brush geometry to become corrupted after multiple save operations.</p>
  {% include download-sf-win.md ver='1.7.3' %}
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 1.7.2</span>
    <span class="date">2012-07-16</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=60 %})</span>
  </h2>
  <p>This release contains a bugfix for a long-lasting but irritating issue whereby entities would be renamed unnecessarily when importing or pasting data into a map.</p>
  {% include download-sf-win.md ver='1.7.2' %}
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 1.7.1</span>
    <span class="date">2012-06-09</span>
  </h2>
  <p>This is a bugfix release containing fixes for a number of outstanding renderer issues and other defects.</p>
  {% include download-sf-win.md ver='1.7.1' %}
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 1.7.0</span>
    <span class="date">2011-11-26</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=53 %})</span>
  </h2>
  <p>With DarkRadiant 1.7.0 a massive list of improvements has been made available, next to the usual long list of bugfixes. A fully-fledged Particle Editor, real-time render preview, increased map loading performance, reduced memory consumption and many improvements related to layers, to name the most important changes over the previous release.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.7.0/darkradiant-1.7.0.x64.exe/download">darkradiant-1.7.0.x64.exe</a></li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.7.0/darkradiant-1.7.0.exe/download">darkradiant-1.7.0.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 1.6.1</span>
    <span class="date">2011-04-23</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=54 %})</span>
  </h2>
  <p>DarkRadiant 1.6.1 is a maintenance or bugfix release which resolves a few issues that came up since 1.6.0.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.6.1/darkradiant-1.6.1.x64.exe/download">darkradiant-1.6.1.x64.exe</a></li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.6.1/darkradiant-1.6.1.exe/download">darkradiant-1.6.1.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 1.6.0</span>
    <span class="date">2011-04-08</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=50 %})</span>
  </h2>
  <p>DarkRadiant 1.6.0 introduces native support for the Quake 4 Map Format as well as a rudimentary quake4.game definition (to be tested, feedback is welcome). The 3D renderer went through some profiling and	is operating considerably faster now.  A few bugs and crashes have been fixed as well.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.6.0/darkradiant-1.6.0.x64.exe/download">darkradiant-1.6.0.x64.exe</a></li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.6.0/darkradiant-1.6.0.exe/download">darkradiant-1.6.0.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 1.5.0</span>
    <span class="date">2011-01-21</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=48 %})</span>
  </h2>
  <p>As most prominent feature DarkRadiant 1.5.0 provides a newly written Particle Previewer, including real-time particle rendering. Besides a few bugfixes and usability improvements, the major changes happened behind the scenes (all the UI code has been refactored to use GTK's C++ interface gtkmm).</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.5.0/darkradiant-1.5.0.x64.exe/download">darkradiant-1.5.0.x64.exe</a></li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.5.0/darkradiant-1.5.0.exe/download">darkradiant-1.5.0.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 1.4.0</span>
    <span class="date">2010-07-21</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=45 %})</span>
  </h2>
  <p>The 1.4.0  release introduces a small set of new features, including Selection Sets, a new Group Part selection mode, Vocal Set Chooser (for TDM 1.03+) and a couple of bugfixes.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.4.0/darkradiant-1.4.0.x64.exe/download">darkradiant-1.4.0.x64.exe</a></li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.4.0/darkradiant-1.4.0.exe/download">darkradiant-1.4.0.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 1.3.2</span>
    <span class="date">2010-06-20</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=46 %})</span>
  </h2>
  <p>This is a bugfix release, resolving a couple of issues related to filtering, decal rendering and curve handling.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.3.2/darkradiant-1.3.2.x64.exe/download">darkradiant-1.3.2.x64.exe</a></li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.3.2/darkradiant-1.3.2.exe/download">darkradiant-1.3.2.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 1.3.1</span>
    <span class="date">2010-05-30</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=44 %})</span>
  </h2>
  <p>This is a bugfix release superseding the recently published 1.3.0 feature release, resolving a few annoying crashes related to the Objectives Editor plug-in. No new features have been introduced, except for the ability to select the camera position in Splitpane layout.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.3.1/darkradiant-1.3.1.x64.exe/download">darkradiant-1.3.1.x64.exe</a></li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.3.1/darkradiant-1.3.1.exe/download">darkradiant-1.3.1.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 1.3.0</span>
    <span class="date">2010-05-25</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=38 %})</span>
  </h2>
  <p>This feature release introduces support for multiple languages. German is included as first &quot;foreign&quot; language - if you're interested in translating DarkRadiant into your language, feel free to contact us.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.3.0/darkradiant-1.3.0.x64.exe/download">darkradiant-1.3.0.x64.exe</a></li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.3.0/darkradiant-1.3.0.exe/download">darkradiant-1.3.0.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 1.2.2</span>
    <span class="date">2010-04-19</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=42 %})</span>
  </h2>
  <p>This is a regular maintenance/bugfix release, resolving some crashes and adding support for automatically disabling Windows desktop composition on startup.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.2.2/darkradiant-1.2.2.x64.exe/download">darkradiant-1.2.2.x64.exe</a></li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.2.2/darkradiant-1.2.2.exe/download">darkradiant-1.2.2.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 1.2.1</span>
    <span class="date">2010-03-16</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=40 %})</span>
  </h2>
  <p>A critical bug surfaced in the recently released 1.2.0 preventing fonts in PK4 files from being recognised by DarkRadiant's readable editor.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.2.1/darkradiant-1.2.1.x64.exe/download">darkradiant-1.2.1.x64.exe</a></li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.2.1/darkradiant-1.2.1.exe/download">darkradiant-1.2.1.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 1.2.0</span>
    <span class="date">2010-03-12</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=37 %})</span>
  </h2>
  <p>The most prominent feature in this release is the newly written <strong>Readable Editor</strong> plugin, making WYSIWYG editing of The Dark Mod readables finally possible.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.2.0/darkradiant-1.2.0.x64.exe/download">darkradiant-1.2.0.x64.exe</a></li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.2.0/darkradiant-1.2.0.exe/download">darkradiant-1.2.0.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 1.1.0</span>
    <span class="date">2010-01-16</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=35 %})</span>
  </h2>
  <p>A <strong>massive</strong> list of improvements made it into this release, I  strongly recommend upgrading to the this newest version. New texturing tools are available,  overall performance has been improved, Python scripting support has been enhanced, and a couple of stability and usability changes made it into this release.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.1.0/darkradiant-1.1.0.x64.exe/download">darkradiant-1.1.0.x64.exe</a></li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.1.0/darkradiant-1.1.0.exe/download">darkradiant-1.1.0.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 1.0.2</span>
    <span class="date">2009-10-26</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=34 %})</span>
  </h2>
  <p>The critical bug surfaced in the recently released 1.0.0 was still not fixed in 1.0.1 hence a new bugfix release was in order.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.0.2/darkradiant-1.0.2.x64.exe/download">darkradiant-1.0.2.x64.exe</a></li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.0.2/darkradiant-1.0.2.exe/download">darkradiant-1.0.2.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 1.0.1</span>
    <span class="date">2009-10-24</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=31 %})</span>
  </h2>
  <p>A critical bug surfaced in the recently released 1.0.0 which crashed the application on cloning patches. This has been fixed, as long with two other minor bugs.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.0.1/darkradiant-1.0.1.x64.exe/download">darkradiant-1.0.1.x64.exe</a></li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.0.1/darkradiant-1.0.1.exe/download">darkradiant-1.0.1.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 1.0.0</span>
    <span class="date">2009-10-16</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=30 %})</span>
  </h2>
  <p>After three years of development DarkRadiant 1.0.0 finally sees the light of day.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.0.0/darkradiant-1.0.0.x64.exe/download">darkradiant-1.0.0.x64.exe</a></li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.0.0/darkradiant-1.0.0.exe/download">darkradiant-1.0.0.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.10.0</span>
    <span class="date">2009-06-21</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=29 %})</span>
  </h2>
  <p>DarkRadiant 0.10.0 includes an upgraded render and shader system, to improve support for id tech 4 materials and to give a better preview of maps in lighting mode. This point release also resolves some problems observed on multi-monitor setups.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.10.0/darkradiant-0.10.0.x64.exe/download">darkradiant-0.10.0.x64.exe</a></li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.10.0/darkradiant-0.10.0.exe/download">darkradiant-0.10.0.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.9.12</span>
    <span class="date">2009-03-12</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=28 %})</span>
  </h2>
  <p>This is a bugfix release addressing a bug in the shader file parser. Many models using shaders without qer_editorimage expressions were showing up with &quot;shader not found&quot;. This supercedes the previous release, as usual.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.9.12/darkradiant-0.9.12.x64.exe/download">darkradiant-0.9.12.x64.exe</a></li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.9.12/darkradiant-0.9.12.exe/download">darkradiant-0.9.12.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.9.11</span>
    <span class="date">2009-03-09</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=27 %})</span>
  </h2>
  <p>This release features a newly written command system under the hood - DarkRadiant has its own command console now, making it possible to fire operations by typing and to create new command aliases and &quot;binds&quot;.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.9.11/darkradiant-0.9.11.x64.exe/download">darkradiant-0.9.11.x64.exe</a></li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.9.11/darkradiant-0.9.11.exe/download">darkradiant-0.9.11.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.9.10</span>
    <span class="date">2009-02-06</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=26 %})</span>
  </h2>
  <p>There have been a few bugfixes, many usability improvements and better DEF file parsing support as well as a newprefab preview window.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.9.10/darkradiant-0.9.10.x64.exe/download">darkradiant-0.9.10.x64.exe</a></li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.9.10/darkradiant-0.9.10.exe/download">darkradiant-0.9.10.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.9.9</span>
    <span class="date">2008-12-30</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=23 %})</span>
  </h2>
  <p>DarkRadiant 0.9.9 includes a lot of noticeable improvements, including improved DDS texture handling, better memory consumption, new GUIs and lots of bugfixes and usability changes. This release is also the first one including a build targetting the Windows x64 platform (Vista 64).</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.9.9/darkradiant-0.9.9.1.x64.exe/download">darkradiant-0.9.9.1.x64.exe</a></li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.9.9/darkradiant-0.9.9.1.exe/download">darkradiant-0.9.9.1.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.9.8</span>
    <span class="date">2008-12-07</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=22 %})</span>
  </h2>
  <p>Contains tons of fixes and a new Conversation Editor GUI to facilitate editing dialogs in DarkMod maps.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.9.8/darkradiant-0.9.8.1.exe/download">darkradiant-0.9.8.1.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.9.7</span>
    <span class="date">2008-08-29</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=20 %})</span>
  </h2>
  <p>Contains a number of bugfixes, a rewritten namespace and a new Objectives GUI to facilitate editing objectives in DarkMod maps.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.9.7/darkradiant-0.9.7.exe/download">darkradiant-0.9.7.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.9.6</span>
    <span class="date">2008-04-06</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=16 %})</span>
  </h2>
  <p>Contains a number of bugfixes, support for layers and a Difficulty Editor GUI specifically for editing DarkMod-maps.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.9.6/darkradiant-0.9.6.exe/download">darkradiant-0.9.6.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.9.5</span>
    <span class="date">2008-01-19</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=15 %})</span>
  </h2>
  <p>Further improves the support for MD5 models and skins. A new plug-in has been developed to allow issuing &quot;dmap&quot; commands to a running TDM instance.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.9.5/darkradiant-0.9.5.exe/download">darkradiant-0.9.5.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.9.4</span>
    <span class="date">2007-11-02</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=12 %})</span>
  </h2>
  <p>This is a bugfix release addressing an issue with the inheritance of  entity classes in the Entity Browser, with a couple of other tweaks.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.9.4/darkradiant-0.9.4.exe/download">darkradiant-0.9.4.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.9.3</span>
    <span class="date">2007-10-21</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=11 %})</span>
  </h2>
  <p>This is a minor release with a couple of bugfixes and tweaks, and is  also the first release which contains the refactored module system.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.9.3/darkradiant-0.9.3.exe/download">darkradiant-0.9.3.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.9.2</span>
    <span class="date">2007-09-06</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=10 %})</span>
  </h2>
  <p>This release adds support of CurveNURBS and CurveCatmullROM control vertex editing, better Doom 3 shader support (<em>addnormals</em> and other MapExpressions, built-in textures like <em>_white</em>, etc.), a mod-based grouping of the elements in the Entity Chooser and many other bugfixes, tweaks, usability and performance improvements.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.9.2/darkradiant-0.9.2.exe/download">darkradiant-0.9.2.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.9.1</span>
    <span class="date">2007-06-10</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=9 %})</span>
  </h2>
  <p>New in this release: SoundShader playback, improved handling of func_* entities, draggable func_* origin, <em>Add/Move Player Start here</em> option in context menu, fixed and improved patch vertex commands (Add/Delete/Append patch columns/rows) and a new <em>Select Children</em> command.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.9.1/darkradiant-0.9.1.exe/download">darkradiant-0.9.1.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.9.0</span>
    <span class="date">2007-04-29</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=3 %})</span>
  </h2>
  <p>This release contains a massive amount of improvements, refer to the changelog.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.9.0/darkradiant-0.9.0.exe/download">darkradiant-0.9.0.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.8.1</span>
    <span class="date">2007-01-28</span>
  </h2>
  <p>This release fixes a few major bugs discovered in the previous release.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.8.1/darkradiant-0.8.1.exe/download">darkradiant-0.8.1.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.8.0</span>
    <span class="date">2007-01-26</span>
    <span class="changelog">({% include bugtracker_changelog_link.md version=4 %})</span>
  </h2>
  <p>A couple of new features made it into this release, like a new LightInspector and the support for projected lights. New texturing tools and a skin chooser are available among other things.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.8.0/darkradiant-0.8.0.exe/download">darkradiant-0.8.0.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.7.1</span>
    <span class="date">2006-11-26</span>
  </h2>
  <p>Contains an improved Filter System, a new Media Browser, customisable colour schemes and numerous improvements over the previous release.</p>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.7.1/darkradiant-0.7.1.exe/download">darkradiant-0.7.1.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.7.0</span>
    <span class="date">2006-11-05</span>
  </h2>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.7.0/darkradiant-0.7.0.exe/download">darkradiant-0.7.0.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.6.0</span>
    <span class="date">2006-09-29</span>
  </h2>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.6.0/darkradiant-0.6.0.exe/download">darkradiant-0.6.0.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.5.3</span>
    <span class="date">2006-08-25</span>
  </h2>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.5.3/darkradiant-0.5.3.exe/download">darkradiant-0.5.3.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.5.2</span>
    <span class="date">2006-08-18</span>
  </h2>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.5.2/darkradiant-0.5.2.exe/download">darkradiant-0.5.2.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.5.1</span>
    <span class="date">2006-07-23</span>
  </h2>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.5.1/darkradiant-0.5.1.exe/download">darkradiant-0.5.1.exe (32-Bit)</a></li>
  </ul>
</div>

<div class="section download">
  <h2>
    <span class="">DarkRadiant 0.5.0</span>
    <span class="date">2006-07-16</span>
  </h2>
  <h3>Windows Installer</h3>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/0.5.0/darkradiant-0.5.0.exe/download">darkradiant-0.5.0.exe (32-Bit)</a></li>
  </ul>
</div>
