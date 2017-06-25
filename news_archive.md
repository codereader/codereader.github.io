---
layout: default
title: DarkRadiant News Archive
---
<div class="section">
  <h2>
    <span class="date">2014-07-14</span>
    <span class="title">DarkRadiant 1.8.1 released</span>
  </h2>
  <p>This release contains a couple of bug fixes and some new functionality. View the full list of fixes on our {% include bugtracker_changelog_link.md version=64 %}.</p>
  <p class="important">Note that you might need to update the VC++ support files, get them here: <a href="http://www.microsoft.com/en-US/download/details.aspx?id=30679">VC++ 2012 Redistributable Package (all platforms)</a></p>
  {% include download-sf-win.md ver='1.8.1' %}
  {% include download-linux.md ver='1.8.1' %}
</div>

<div class="section">
  <h2>
    <span class="date">2013-10-12</span>
    <span class="title">DarkRadiant 1.8.0 released</span>
  </h2>
  <p>This release contains numerous bug and stability fixes as well as one new feature for flooring objects. Some improvements have also been made to better support different game types. View the full list of fixes on our {% include bugtracker_changelog_link.md version=57 %}.</p>
  {% include download-sf-win.md ver='1.8.0' %}
  {% include download-linux.md ver='1.8.0' %}
</div>

<div class="section">
  <h2>
    <span class="date">2013-02-02</span>
    <span class="title">DarkRadiant 1.7.3 released</span>
  </h2>
  <p>This release contains a fix for a subtle but serious data corruption bug which caused non-worldspawn brush geometry to become corrupted after multiple save operations.</p>
  {% include download-sf-win.md ver='1.7.3' %}
  {% include download-linux.md ver='1.7.3' %}
</div>

<div class="section">
  <h2>
    <span class="date">2012-07-16</span>
    <span class="title">DarkRadiant 1.7.2 released</span>
  </h2>
  <p>This release contains a bugfix for a long-lasting but irritating issue whereby entities would be renamed unnecessarily when importing or pasting data into a map.</p>
  {% include download-sf-win.md ver='1.7.2' %}
  {% include download-linux.md ver='1.7.2' %}
</div>

<div class="section">
  <h2>
    <span class="date">2012-06-09</span>
    <span class="title">DarkRadiant 1.7.1 released</span>
  </h2>
  <p>This is a bugfix release containing fixes for a number of outstanding renderer issues and other defects, including: 
  <ul>
        <li>Fixed black render artifacts in model preview window (#2939).</li>
        <li>Fixed lighting view turning black when certain models are in view
        (#2969).</li>
        <li>Fixed crash on exit after changing view layout (#2954).</li>
        <li>Fixed sky box textures failing to render.</li>
        <li>Fixed inability to move vertices with arrow keys in camera view
        (#2938).</li>
        <li>Fixed crash after Save As in Particle Editor (now renamed to Copy to
        better reflect its behaviour).</li>
        <li>Fixed crash in Readables editor if certain font resources were
        missing from the mod assets tree.</li>
        <li>Re-designed model chooser allows control over visibility of model's
        component materials.</li>
        <li>Improved performance of map loading and population of certain asset
        tree views (#2987).</li>
        <li>Splitter position in certain dialogs is persistent.</li>
        <li>Linux build does not fail if GtkSourceView is not available, this is
        now an optional dependency.</li>
        <li>Updated GTK and related library versions on Windows (#2945)</li>
      </ul></p>
  {% include download-sf-win.md ver='1.7.1' %}
  {% include download-linux.md ver='1.7.1' %}
</div>

<div class="section">
  <h2>
    <span class="date">2012-05-03</span>
    <span class="title">DarkRadiant source now hosted on Github</span>
  </h2>
  <p>Users who build DarkRadiant from source should be aware that the source code is now being hosted on Github rather than SourceForge SVN. See the <a href="source.html">Source code</a> page for information about setting up Git and accessing the repository.</p>
  <p>The existing SourceForge SVN repository will remain available and will continue to host the dependencies directories for building on Windows, however the SVN trunk will no longer be updated with changes to the DarkRadiant application.</p>
</div>

<div class="section">
  <h2>
    <span class="date">2011-04-23</span>
    <span class="title">DarkRadiant 1.6.1 available</span>
  </h2>
  <p>DarkRadiant 1.6.1 is a maintenance or bugfix release which resolves a few issues that came up since 1.6.0.</p>
      <p class="subheadline">Important</p>
      <p>Starting with this release the Windows build is compiled using VC++ 2010, so be sure to install the <strong>VC++ 2010</strong> redistributable package in order to run this release:
  <ul>
    <li><a href="http://www.microsoft.com/downloads/en/details.aspx?familyid=A7B7A05E-6DE6-4D3A-A423-37BF0912DB84&displaylang=en">VC++ 2010 Redistributable Package 32 Bit</a></li>
    <li><a href="http://www.microsoft.com/downloads/en/details.aspx?displaylang=en&FamilyID=bd512d9e-43c8-4655-81bf-9350143d5867">VC++ 2010 Redistributable Package 64 Bit</a></li>
  </ul>
  </p>
      <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
      <p class="subheadline">Windows 32-bit</p>
      <ul>
        <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.6.1/darkradiant-1.6.1.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
        <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.6.1/darkradiant-1.6.1.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows 32-bit) </li>
      </ul>
      <p class="subheadline">Windows 64-bit</p>
      <ul>
        <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.6.1/darkradiant-1.6.1.x64.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
        <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.6.1/darkradiant-1.6.1.x64.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows x64) </li>
      </ul>
      <p class="subheadline">Ubuntu / Kubuntu Linux</p>
      <ul>
        <li>Please follow the instructions on our <a href="https://launchpad.net/~orbweaver/+archive/darkradiant">Launchpad page</a> to download a DarkRadiant package for Ubuntu.</li>
      </ul>
</div>

<div class="section">
  <h2>
    <span class="date">2011-04-08</span>
    <span class="title">DarkRadiant 1.6.0 available</span>
  </h2>
  <p>DarkRadiant 1.6.0 introduces native support for the Quake 4 Map Format as well as a rudimentary quake4.game definition (to be tested, feedback is welcome). The 3D renderer went through some profiling and
  is operating considerably faster now. A few bugs and crashes have been fixed as well.</p>
      <p class="subheadline">Important</p>
      <p>Starting with this release the Windows build is compiled using VC++ 2010, so be sure to install the <strong>VC++ 2010</strong> redistributable package in order to run this release:
  <ul>
    <li><a href="http://www.microsoft.com/downloads/en/details.aspx?familyid=A7B7A05E-6DE6-4D3A-A423-37BF0912DB84&displaylang=en">VC++ 2010 Redistributable Package 32 Bit</a></li>
    <li><a href="http://www.microsoft.com/downloads/en/details.aspx?displaylang=en&FamilyID=bd512d9e-43c8-4655-81bf-9350143d5867">VC++ 2010 Redistributable Package 64 Bit</a></li>
  </ul>
  </p>
      <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
      <p class="subheadline">Windows 32-bit</p>
      <ul>
        <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.6.0/darkradiant-1.6.0.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
        <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.6.0/darkradiant-1.6.0.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows 32-bit) </li>
      </ul>
      <p class="subheadline">Windows 64-bit</p>
      <ul>
        <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.6.0/darkradiant-1.6.0.x64.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
        <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.6.0/darkradiant-1.6.0.x64.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows x64) </li>
      </ul>
      <p class="subheadline">Ubuntu / Kubuntu Linux</p>
      <ul>
        <li>Please follow the instructions on our <a href="https://launchpad.net/~orbweaver/+archive/darkradiant">Launchpad page</a> to download a DarkRadiant package for Ubuntu.</li>
      </ul>
</div>

<div class="section">
  <h2>
    <span class="date">2011-01-21</span>
    <span class="title">DarkRadiant 1.5.0 released</span>
  </h2>
  <p>As most prominent feature DarkRadiant 1.5.0 provides a newly written Particle Previewer, including real-time particle rendering. Besides a few bugfixes and usability improvements, the major changes happened behind the scenes (all the UI code has been refactored to use GTK's C++ interface gtkmm).</p>
  <p align="left"><a href="images/screenshots/particle_preview01.png"><img src="images/screenshots/particle_preview01_small.png" alt="Particle Previewer" /></a></p>
      <p class="subheadline">Important</p>
      <p>Starting with this release the Windows build is compiled using VC++ 2010, so be sure to install the <strong>VC++ 2010</strong> redistributable package in order to run this release:
  <ul>
    <li><a href="http://www.microsoft.com/downloads/en/details.aspx?familyid=A7B7A05E-6DE6-4D3A-A423-37BF0912DB84&displaylang=en">VC++ 2010 Redistributable Package 32 Bit</a></li>
    <li><a href="http://www.microsoft.com/downloads/en/details.aspx?displaylang=en&FamilyID=bd512d9e-43c8-4655-81bf-9350143d5867">VC++ 2010 Redistributable Package 64 Bit</a></li>
  </ul>
  </p>
  <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
  <p class="subheadline">Windows 32-bit</p>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.5.0/darkradiant-1.5.0.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.5.0/darkradiant-1.5.0.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows 32-bit) </li>
  </ul>
  <p class="subheadline">Windows 64-bit</p>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.5.0/darkradiant-1.5.0.x64.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.5.0/darkradiant-1.5.0.x64.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows x64) </li>
  </ul>
  <p class="subheadline">Ubuntu / Kubuntu Linux</p>
  <ul>
    <li>Please follow the instructions on our <a href="https://launchpad.net/~orbweaver/+archive/darkradiant">Launchpad page</a> to download a DarkRadiant package for Ubuntu.</li>
  </ul>
</div>

<div class="section">
  <h2>
    <span class="date">2010-07-21</span>
    <span class="title">DarkRadiant 1.4.0 released</span>
  </h2>
  <p>The 1.4.0  release introduces a small set of new features, including Selection Sets, a new Group Part selection mode, Vocal Set  Chooser (for TDM 1.03+) and a couple of bugfixes.</p>
  <p class="subheadline">Important</p>
  <p>Be sure to install  the <strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en" target="_blank">VC++ 2008</a></strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en"> redistributable package</a> in order to run this release. </p>
  <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
  <p class="subheadline">Windows 32-bit</p>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.4.0/darkradiant-1.4.0.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.4.0/darkradiant-1.4.0.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows 32-bit) </li>
  </ul>
  <p class="subheadline">Windows 64-bit</p>
  <ul>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.4.0/darkradiant-1.4.0.x64.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
    <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.4.0/darkradiant-1.4.0.x64.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows x64) </li>
  </ul>
  <p class="subheadline">Ubuntu / Kubuntu Linux</p>
  <ul>
    <li>Please follow the instructions on our <a href="https://launchpad.net/~orbweaver/+archive/darkradiant">Launchpad page</a> to download a DarkRadiant package for Ubuntu.</li>
  </ul>
</div>
