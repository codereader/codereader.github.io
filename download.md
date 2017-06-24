---
layout: default
title: DarkRadiant, open-source level editor for Doom 3 and The Dark Mod
---
<table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 2.2.1</th>
      <th width="150" class="note">2017-02-07</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td><p>
        This is a feature release containing a few bugifxes and stabilisations. It's recommended to prefer this release over any previous ones.
      </p>
	  <p class="subheadline">Changes</p>
      <ul>
		    <li>Ability to scale models</li>
			<li>Added Measurement tool for distance</li>
			<li>Rotation manipulator's pivot point is moveable now</li>
			<li>Added support for shift/scale/rotation keywords of ASE model</li>
			<li>Added ability to snap rotation origin to grid</li>
			<li>Added Layer Usage Breakdown tab to Map Info Dialog</li>
			<li>Added indicator to Layer Dialog to show whether anything in the current selection is part of this layer</li>
			<li>Added option to validate that Conversation actors are existing in the map</li>
			<li>Conversation Editor GUI Improvements</li>
			<li>Colour of grouped objects should be customisable</li>
			<li>Enabled compilation in Mac OS X</li>
			<li>Rewrote MenuManager implementation</li>
			<li>Fixed: Readable Editor refusing to save xdata file if fs_game is set to an absolute path</li>
			<li>Fixed: Readable Editor not marking the map as modified after hitting "Save and Close"</li>
			<li>Fixed: Worldspawn is not saved as Entity 0 in some scenarios</li>
			<li>Fixed: DarkRadiant crashes when "Load last map" option is active</li>
			<li>Fixed: Tons of g++ 6.2 compiler warnings</li>
			<li>Fixed: Making all in install/i18n fails when gettext binaries are missing</li>
			<li>Fixed: Clicking Entity Pane Columns Messes Up Spawnarg Order</li>
			<li>Fixed: Crash at startup in std::string constructor (g++ 5.3)</li>
			<li>Fixed: LayerControlDialog's Hide/Show All button is not graying out correctly</li>
			<li>Fixed: crash in boost::phyton</li>
			<li>Fixed: Rare crash opening Texture Tool</li>
			<li>Fixed: Layer submenu items in OrthoContextmenu not working in wxGTK</li>
			<li>Fixed: Stim/Response Editor partly doesn't work, also crashes DarkRadiant</li>
			<li>Fixed: Crash when closing S/R editor in Linux</li>
			<li>Fixed: Crash in S/R ClassEditor when right-clicking a Response (Linux)</li>
			<li>Fixed: Startup warning "unable to create settings path" in Linux</li>
			<li>Fixed: Crash during shutdown due to resources still held by S/R module</li>
			<li>Fixed: Problem Playing Speaker Sounds in Entity Inspector Choose Sound Dialog.</li>
			<li>Fixed: Sound Chooser doesn't preselect the shader when editing a s_shader spawnarg</li>
			<li>Fixed: Build failure on Arch Linux</li>
			<li>Fixed: Linux './configure' script WARNING</li>
			<li>Fixed: Linux build failure</li>
			<li>Fixed: Crash due to concurrent XMLRegistry accesses from multiple threads</li>
			<li>Fixed: Removing worldspawn from the map prevents new brushes from being drag-created</li>
       </ul>
      <p class="subheadline">Windows</p>
      <ul>
        <li><a href="https://github.com/codereader/DarkRadiant/releases/download/2.2.1/darkradiant-2.2.1-x64.exe"><strong>Download</strong></a> (Installer, Windows x64)</li>
        <li><a href="https://github.com/codereader/DarkRadiant/releases/download/2.2.1/darkradiant-2.2.1-x86.exe"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
      </ul>
      <p class="subheadline">Linux</p>
      <p>
        Packages are made available by the Debian Games group, these are usually available in the Ubuntu Software Center after some delay.
      </p></td>
    </tr>
  </table>

  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 2.1.0</th>
      <th width="150" class="note">2016-11-18</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td><p>
        This is a feature release containing a few bugifxes and stabilisations. It's recommended to prefer this release over any previous ones.
      </p>
	  <p class="subheadline">Changes</p>
      <ul>
		    <li>Switched Windows toolchain to Visual C++ 2015</li>
			<li>Updated backend libraries</li>
			<li>Grouping</li>
			<li>Ported patch tesselation code from idtech4, completely replacing the one in DR</li>
			<li>Fixed the Objectives Numbers not being rendered in the list (Objectives Editor)</li>
			<li>Added AAS File Visualisation. The dialog is available through the "View" menu and/or by pressing Ctrl-Shift-A (default mapping)</li>
			<li>Added feature to Pan the camera view by clicking Ctrl-RMB and dragging (#4333: 3d view port shortcut to pan while not in free look)</li>
			<li>Double-clicking tree view items now expands/collapses them</li>
			<li>Fixed #4325: Empty func_static entity after switching classname and hitting undo</li>
			<li>Fixed #4280: Aspect ratio displayed incorrectly in particle editor</li>
			<li>Fixed: MoveSelectionUP command crashing DR when nothing is selected</li>
			<li>Tons of refactorings and back-end stuff</li>
			<li>Fixed various compilation errors in Linux</li>
			<li>Fixed #4355: Problem with starting a new conversation with the conversation editor</li>
			<li>Fixed #4375: Moving objects to a hidden layer doesn't cause them to immediately disappear</li>
			<li>Fixed #4373: Connecting lines are created in Default layer</li>
			<li>Feature #4380: Allow EntityInspector to select/copy/paste multiple spawnargs at once</li>
			<li>Feature #4381: Add a clickable Checkbox next to boolean-valued spawnargs in EntityInspector list</li>
			<li>Fixed #4386: Projected lights don't rotate around their origin anymore</li>
			<li>Fixed #4373: Connecting lines are created in Default layer. Also, target lines of cloned nodes might appear hidden at first.</li>
			<li>Fixed #4391: Aimed particles have incorrect orientation or shape</li>
			<li>Fixed #4365: a few static warnings (llvm/clang static source code analysis)</li>
			<li>Fixed #4404: The health field on the AI tab is capped at 1000.</li>
			<li>Added script to check for invalid visportals (i.e. portals with more than one sided textured with textures/editor/visportal)</li>
			<li>Fixed #4410: Particle distribution parameters not saved to the .prt file (ring parameter for spherical particles)</li>
			<li>Fixed #3870: Number of selected map items is now shown in the status bar</li>
       </ul>
      <p class="subheadline">Windows</p>
      <ul>
        <li><a href="https://github.com/codereader/DarkRadiant/releases/download/2.1.0/darkradiant-2.1.0-x64.exe"><strong>Download</strong></a> (Installer, Windows x64)</li>
        <li><a href="https://github.com/codereader/DarkRadiant/releases/download/2.1.0/darkradiant-2.1.0-x86.exe"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
      </ul>
      <p class="subheadline">Linux</p>
      <p>
        Packages will be published in the <a href="https://launchpad.net/~orbweaver/+archive/darkradiant">Launchpad PPA</a> shortly.
      </p></td>
    </tr>
  </table>

  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 2.0.4</th>
      <th width="150" class="note">2016-06-04</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td><p>
        This is a bugifx/stabilisation release including a few nice additions. It's recommended to prefer this release over any previous ones.
      </p>
	  <p class="subheadline">Changes</p>
      <ul>
		    <li>[Map Editing] Patches + Incorrect Shader Paste operations breaks the 3D viewport</li>
			<li>[Saving and loading] Add support for loading older Q3 map format</li>
			<li>[GUI] Increasing/decreasing camera speed during freelook mode exits freelook</li>
			<li>[GUI] Color-related spawnargs should have three points of decimal precision instead of two</li>
			<li>[Scripting] Move Wavefront OBJ exporter code to Python</li>
			<li>[GUI] Moving texture/vert points in texture tool: always moves two grid lines at a time</li>
			<li>[Design/Coding] Path connections disappear when one endpoint is not visible</li>
			<li>[GUI] Delay redraw when manipulating brushes or patches</li>
			<li>[GUI] Have to double click to select and unselect any item on ortho.</li>
			<li>[Map Editing] Multiple func_statics, when rotated, leave origins untouched</li>
			<li>[Design/Coding] Animation viewer keeps demanding more memory</li>
			<li>[Design/Coding] Crash when reloading def files while having a map loaded</li>
			<li>[GUI] Cannot set negative speed values in particle editor</li>
			<li>[GUI] The AI tab shows visual AND audio acuities ranging from 0->1.00. They should range from 0->100.</li>
			<li>[Map Editing] Find and replace textures ignores texture alignment</li>
			<li>[Map Editing] Crash when selecting an object after loading a new map</li>
			<li>[Map Editing] Rotation of multi-ent objects problematic</li>
      </ul>
      <p class="subheadline">Windows</p>
      <ul>
        <li><a href="https://github.com/codereader/DarkRadiant/releases/download/2.0.4/darkradiant-2.0.4-x64.exe"><strong>Download</strong></a> (Installer, Windows x64)</li>
        <li><a href="https://github.com/codereader/DarkRadiant/releases/download/2.0.4/darkradiant-2.0.4-x86.exe"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
      </ul>
      <p class="subheadline">Linux</p>
      <p>
        Packages will be published in the <a href="https://launchpad.net/~orbweaver/+archive/darkradiant">Launchpad PPA</a> shortly.
      </p></td>
    </tr>
  </table>

  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 2.0.3</th>
      <th width="150" class="note">2015-12-30</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td><p>
        This is a bugifx/stabilisation release. It's recommended to prefer this release over the recent 2.0.2.
      </p>
	  <p class="subheadline">Changes</p>
      <ul>
		    <li>[Renderer] Portal Sky texture is transparent (again)</li>
			<li>[GUI] Crash in Freezepointer code, during ParticlesChooser</li>
			<li>[General] configure.ac: needs call to AM_GNU_GETTEXT_VERSION, does not find de.po</li>
			<li>[Shader System] texture browser not updating on media load</li>
			<li>[GUI] Startup crash in release builds when .pid-file is present</li>
			<li>[General] please update boost.m4 to avoid build failure with gcc-5</li>
			<li>[Design/Coding] Please add Keywords to desktop file</li>
			<li>[GUI] STIM_MOSS not listed in S/R editor</li>
			<li>[General] spelling error in sound module</li>
			<li>[Models] Reload models unhides hidden models</li>
			<li>[Models] Changing model on an entity with a skin reverts skin to default</li>
			<li>[Map Editing] Feature request: saved paths in prefab inspector</li>
			<li>[GUI] TextureBrowser Setting "Max shadername length" ignored in Preferences</li>
			<li>[Selection System] 'select group parts' toolbar button stuck</li>
			<li>[GUI] Readable Editor not working in SplitPane layout</li>
			<li>[Design/Coding] Rare crash during startup due to duplicate worker threads</li>
			<li>[Objectives] Instability in Objective Editor</li>
			<li>[Objectives] Objective Component always reverting its value to 1 when selected</li>
			<li>[Map Editing] func_door issues with models</li>
			<li>[Map Editing] Crash when closing an additional XY view window</li>
			<li>[Map Editing] Dragged entity loses angle field</li>
			<li>[Design/Coding] "angle" spawnarg disappears when it's set to zero and the entity is moved</li>
			<li>[Map Editing] Crash when moving single PatchNode over 512 units away from origin</li>
			<li>[GUI] Find and Replace - seek to material</li>
			<li>[GUI] find and replace texture dialog box. using mouse 3</li>
			<li>[GUI] Show the keyboard shortcut in the toolbar button help texts</li>
			<li>[Design/Coding] Startup Performance Improvements</li>
			<li>[Objectives] Objectives Editor should remember its size and position</li>
			<li>[Map Editing] Layers: after "Hide All", showing a single layer doesn't make it the default layer</li>
			<li>[GUI] When clicking on the Layer Control Dialog, the scroll bar jumps to the bottom</li>
			<li>[GUI] Add Find & Replace Textures command to the main menu</li>
			<li>[Models] XreaL: MD3 models are loaded without texture</li>
			<li>[GUI] Preload ModelSelector tree after startup</li>
			<li>[GUI] Light Texture Chooser does not display the currently active texture</li>
			<li>[GUI] ModelSelector forgets last selected model when hitting Cancel</li>
			<li>[GUI] ESC key does not propagate as shortcut when a tool window's text control is focused</li>
			<li>[Map Editing] Add "Select/deselect elements using this shader" to MediaBrowser context menu.</li>
			<li>[Sound System] Slashes in sound shader names / shader file decls problematic</li>
			<li>[GUI] Fit texture spin controls too narrow</li>
			<li>[Scripting] Running non-existent script file crashes DR</li>
			<li>[Models] Choosemodel fails to display models when realtime lights are enabled</li>
			<li>[Map Editing] Improve ModelSelector / RenderPreview navigation and rendering</li>
			<li>[GUI] Text box focus issue when creating new layer</li>
			<li>[General] Texture pane isn't initialized when a new map is started</li>
			<li>[Map Editing] Target Lines are rendered in every preview if names happen to match</li>
      </ul>
      <p class="subheadline">Windows</p>
      <ul>
        <li><a href="https://github.com/codereader/DarkRadiant/releases/download/2.0.3/darkradiant-2.0.3-x64.exe"><strong>Download</strong></a> (Installer, Windows x64)</li>
        <li><a href="https://github.com/codereader/DarkRadiant/releases/download/2.0.3/darkradiant-2.0.3-x86.exe"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
      </ul>
      <p class="subheadline">Linux</p>
      <p>
        Packages will be published in the <a href="https://launchpad.net/~orbweaver/+archive/darkradiant">Launchpad PPA</a> shortly.
      </p></td>
    </tr>
  </table>

  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 2.0.2</th>
      <th width="150" class="note">2015-01-10</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td><p>
        This is a bugifx/stabilisation release. It's recommended to prefer this release over the recent 2.0.1.
      </p>
	  <p class="subheadline">Changes</p>
      <ul>
		    <li>SoundChooser doesn't scroll to the selected sound shader</li>
			<li>EntityInspector doesn't react to type-ahead search</li>
			<li>&quot;Wrong type&quot; error window spam in certain menus</li>
			<li>Any items dragged snap back to original location</li>
			<li>Crash in FaceInstance::selectedChanged(debug build) due to invalid callback</li>
			<li>scene::Node destruction issues, PatchNode destructor never invoked</li>
			<li>Rotated light volume can not be resized properly</li>
			<li>Feature request: Adjustable drag / scrolling speed in orthoview</li>
			<li>Particle editor broken in 2.0.2 pre3</li>
			<li>Texture Tool sometimes not drawing, render area is just grey</li>
			<li>Some mouse operations are breaking when cursor is moved beyond the view</li>
			<li>Redesign mouse interaction code used in 3D - and orthoviews</li>
			<li>Switching on realtime rendering might cause irresponsiveness of Camera</li>
			<li>Many treeviews are not sorting alphabetically</li>
			<li>Drag - manipulated func_statics can go off - screen with only origin left for drawing</li>
			<li>Arrow key events in Preference Dialog get propagated to the main window</li>
			<li>Application getting out of focus when closing inspectors</li>
			<li>Ctrl + Tab sometimes does nothing</li>
			<li>DR not remembering ortho layout of SplitPane View after closing DR</li>
			<li>Need option to browse prefabs from non - FM paths as per DR 1.8.1</li>
			<li>When switching to Group Part selection mode, try to keep func_static selections</li>
			<li>Crash when deleting a selection containing both child primitive and parent entity</li>
			<li>Can't type into the SelectionSet dropdown box.</li>
			<li>Search field in Entity list</li>
			<li>Entity list takes ages to show</li>
			<li>GroupDialog Notebook is referenced by two different wxSizerItems at the same time</li>
			<li>Crash when loading a new map with non - empty entity selection</li>
			<li>Light Shader preview sometimes shows just a grey box</li>
			<li>Activating filters under some conditions crashes DR</li>
      </ul>
      <p class="subheadline">Windows</p>
      <ul>
        <li><a href="https://github.com/codereader/DarkRadiant/releases/download/2.0.2/darkradiant-2.0.2-x64.exe"><strong>Download</strong></a> (Installer, Windows x64)</li>
        <li><a href="https://github.com/codereader/DarkRadiant/releases/download/2.0.2/darkradiant-2.0.2-x86.exe"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
      </ul>
      <p class="subheadline">Linux</p>
      <p>
        Packages will be published in the <a href="https://launchpad.net/~orbweaver/+archive/darkradiant">Launchpad PPA</a> shortly.
      </p></td>
    </tr>
  </table>

  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 2.0.1</th>
      <th width="150" class="note">2014-11-15</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td><p>
        This is a bugifx/stabilisation release. It's recommended to prefer this release over the recent 2.0.0.
      </p>
      <ul>
		    <li>Linux fixes for crashes at shutdown</li>
			<li>DarkRadiant doesn't react when clicking around rather fast (#3887)</li>
			<li>TreeView can sometimes hold bad selection references(#3880)</li>
			<li>SplitPane window layout crashes DR at exit(#3875)</li>
			<li>Crash at shutdown in TextureBrowser::destroyWindow() (#3874)</li>
			<li>Rendering performance improvements for patches(#3890)</li>
			<li>Some performance improvements when selecting stuff with modifiers held</li>
			<li>Minor performance improvements when drawing camera and XY views.</li>
			<li>Fixed horizontal splitpane constantly moving to the right with each application run</li>
			<li>Failure to render textures on models in dr / renderer_test.map(materials using _white as map)</li>
			<li>Precautions in attempt to fix ModelSelector crashing after reloading models and / or declarations.</li>
			<li>Fixed startup arguments which were broken in the pre1 build</li>
			<li>Fixed crash at shutdown prevalent in the pre2 builds</li>
			<li>Fixed crash at shutdown when leaving a texture spawnarg selected in EntityInspector</li>
			<li>Increased toolbar item padding</li>
			<li>Adjusted SurfaceInspector layout</li>
			<li>Adjusted LayerControlDialog layout</li>
			<li>LayerControlDialog state is saved on DR exit</li>
			<li>Prefab Selector showing non - prefab files, plus attempts to open folders</li>
			<li>SkinChooser needs a moveable divider</li>
			<li>Linux fixes</li>
			<li>Selecting "Choose Sound..." in Entity Inspector doesn't select the shader in the tree.</li>
			<li>Some windows are inresponsive to mousewheel events(when not in focus)</li>
			<li>Colour picker has a text box next to it now.</li>
			<li>Colourized playback / stop button images.</li>
			<li>Better minimize behaviour for SurfaceInspector, LightInspector, etc.</li>
			<li>Fixed #3851: backslashes in sound paths were ignored by the sound shader parser</li>
			<li>Added default filter to exclude func_statics</li>
			<li>SurfaceInspector's fit entry boxes have 2 digits by default now</li>
			<li>Improved global shortcut handling(pre8)</li>
			<li>Fixed EntityInspector assertion failure on Linux</li>
			<li>Fixed : SurfaceInspector controls will continue firing their events when moving the mouse away</li>
			<li>More precise keyboard shortcut handling for wxDataViewMainWindow(allow underscores)</li>
      </ul>
      <p class="subheadline">Windows</p>
      <ul>
        <li><a href="https://github.com/codereader/DarkRadiant/releases/download/2.0.1/darkradiant-2.0.1-x64.exe"><strong>Download</strong></a> (Installer, Windows x64)</li>
        <li><a href="https://github.com/codereader/DarkRadiant/releases/download/2.0.1/darkradiant-2.0.1-x86.exe"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
      </ul>
      <p class="subheadline">Linux</p>
      <p>
        Packages will be published in the <a href="https://launchpad.net/~orbweaver/+archive/darkradiant">Launchpad PPA</a> shortly.
      </p></td>
    </tr>
  </table>

  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 2.0.0</th>
      <th width="150" class="note">2014-10-10</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td><p>
        This is a major release, the entire UI code has been migrated from GTK+2 to wxWidgets 3.0. Most of the work went into the migration, but a few features and stability fixes made it into this release nonetheless.
      </p>
      <ul>
		<li>Change: Migrate GTK and GLib code to wxWidgets 3.0 (#3777)</li>
		<li>New feature: Fast/slow camera movement switch (#2381)</li>
		<li>New feature: Add "Paste Texture Name only" to mouse shortcuts (#3795)</li>
		<li>New feature: Selecting a shader in the TextureBrowser should fill the ShaderClipboard with the shader name (#3794)</li>
		<li>New feature: Render wireframe from behind for selected patches (#84)</li>
		<li>Fixed: Light shaders appearing the wrong way around (orientation) in DR campared to in-game (#3359).</li>
		<li>Fixed: Rendering of projected lights is not correct (#272)</li>
		<li>Fixed: Can no longer see edges of selections (#3799)</li>
		<li>Fixed: Filtering entities doesn't deselect them (#3783)</li>
      </ul>
      <p class="subheadline">Windows</p>
      <ul>
        <li><a href="http://sourceforge.net/projects/darkradiant/files/darkradiant/2.0.0/darkradiant-2.0.0-x64.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
        <li><a href="http://sourceforge.net/projects/darkradiant/files/darkradiant/2.0.0/darkradiant-2.0.0-x86.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
      </ul>
      <p class="subheadline">Linux</p>
      <p>
        Packages will be published in the <a href="https://launchpad.net/~orbweaver/+archive/darkradiant">Launchpad PPA</a> shortly.
      </p></td>
    </tr>
  </table>

  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 1.8.1</th>
      <th width="150" class="note">2014-07-14</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td><p>
        This release contains a couple of bug fixes and some new functionality.
      </p>
      <ul>
		<li>New feature: support for xreal detal brushes (#3319)</li>
		<li>New feature: Loading and saving maps in Quake 3 format (#3628)</li>
		<li>New feature: Save dialog should offer option to write map using different format (#3627)</li>
		<li>New feature: Make custom bind commands valid targets for keyboard shortcuts (#3626)</li>
		<li>New feature: Skin Chooser on by default (#2019)</li>
		<li>New feature: Add AI Editing Panel for TDM (#3621)</li>
		<li>New feature: Persist SelectionSets to .darkradiant file (#3638)</li>
		<li>Fixed: Select all models of same type not working anymore (#3690)</li>
		<li>Fixed: 0003718: [Scripting] Script to find missing targets (#3718)</li>
		<li>Fixed: MD5 Anim Viewer doesn't remove models after trying to preview a missing mesh (#3644)</li>
		<li>Fixed: Can't save prefabs (#3650)</li>
		<li>Fixed: Copy/Paste map elements seems to be broken (#3652)</li>
		<li>Fixed: Cannot drag selected child primitives when "tabbing" through a func_static entity (#3642)</li>
		<li>Fixed: Cannot drag selected child primitives when in Group Part selection mode (#3641)</li>
		<li>Fixed: Crash when hiding two or more selected patches while PatchInspector is visible (#3639)</li>
		<li>Fixed: Model Selector shows duplicate (previously selected) model after undo operation (#3637)</li>
		<li>Fixed: Readable editor not accurate WYSIWYG (#3062)</li>
		<li>Fixed: Changing Filters is triggering an Entity List refresh even when it's hidden (#3619)</li>
		<li>Fixed: Game-specific settings might be picked from the wrong .game file (#3618)</li>
      </ul>
      <p class="subheadline">Windows</p>
      <ul>
        <li><a href="http://sourceforge.net/projects/darkradiant/files/darkradiant/1.8.1/darkradiant-1.8.1-x64.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
        <li><a href="http://sourceforge.net/projects/darkradiant/files/darkradiant/1.8.1/darkradiant-1.8.1-x86.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
      </ul>
      <p class="subheadline">Linux</p>
      <p>
        Packages will be published in the <a href="https://launchpad.net/~orbweaver/+archive/darkradiant">Launchpad PPA</a> shortly.
      </p></td>
    </tr>
  </table>

  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 1.8.0</th>
      <th width="150" class="note">2013-10-12</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td><p>
        This release contains numerous bug and stability fixes as well as one new feature for flooring objects. Some improvements have also been made to better support different game types.
      </p>
      <ul>
        <li>Add Floor command to move objects downward until they touch the ground.</li>
        <li>Fixed animation preview (#3305).</li>
        <li>Fixed crash when previewing corrupt model (#3273).</li>
        <li>Absolute paths should be supported for game-, mod-path etc. (#3480)</li>
        <li>GameManager adds duplicates VFS search dirs (#2996).</li>
        <li>Cancel-Button in the Preferences-dialog does not work. (#3245)</li>
        <li>Renamed Reload Shaders in File menu as it didn't reflect actual functionality.</li>
        <li>TDM Editing: Objective States INVALID and FAILED are reversed. (#3253)</li>
        <li>Support for pk3dir/pk4dir (#2971)</li>
        <li>TDM Editing: Stim/Response Menu. The "Remove" button is acting like an "Add" button (#3237)</li>
        <li>Two textfields in the DR-preferences don't show text upon start (#3242)</li>
        <li>TDM Editing: Readable Editor creates XData file duplicates in certain cases (#3243)</li>
		<li>Fixed: Minimizing Console window minimizes Dark Radiant (#2942)</li>
		<li>TDM Editing: Stim/Response menu. &quot;Type&quot; List repeats 3 times (#3236)</li>
		<li>Select All of Type (Shift-A) improvements (#3246)</li>
		<li>Remove restriction of having exactly one brush selected when constructing a brush prefab (#3247)</li>
		<li>Particle preview does not render textures (#3061)</li>
		<li>XreaL Editing: Entity > Classname > Choose entity class *Segmentation Fault*</li>
		<li>Surface Inspector: Vertical Scale has wrong German translation (#3030)</li>
		<li>Strange render artefacts in model viewer (#2939)</li>
		<li>Grid text is not rendered (#2951)</li>
		<li>Arrows for manipulating objects not working in Camview (#2938)</li>
		<li>Perform MediaBrowser population code in separate thread (#2987)</li> 
      </ul>
      <p class="subheadline">Windows</p>
      <ul>
        <li><a href="http://sourceforge.net/projects/darkradiant/files/darkradiant/1.8.0/darkradiant-1.8.0-x64.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
        <li><a href="http://sourceforge.net/projects/darkradiant/files/darkradiant/1.8.0/darkradiant-1.8.0-x86.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
      </ul>
      <p class="subheadline">Linux</p>
      <p>
        Packages will be published in the <a href="https://launchpad.net/~orbweaver/+archive/darkradiant">Launchpad PPA</a> shortly.
      </p></td>
    </tr>
  </table>
  
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 1.7.1</th>
      <th width="150" class="note">2012-06-09</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td><p>
        This is a bugfix release containing fixes for a number of outstanding
        renderer issues and other defects, including:
      </p>
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
      </ul>
      <p class="subheadline">Windows</p>
      <ul>
        <li><a href="http://sourceforge.net/projects/darkradiant/files/darkradiant/1.7.1/darkradiant-1.7.1-x64.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
        <li><a href="http://sourceforge.net/projects/darkradiant/files/darkradiant/1.7.1/darkradiant-1.7.1-x86.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
      </ul>
      <p class="subheadline">Linux</p>
      <p>
        Packages will be published in the <a href="https://launchpad.net/~orbweaver/+archive/darkradiant">Launchpad PPA</a> shortly.
      </p></td>
    </tr>
  </table>

  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 1.7.0</th>
      <th width="150" class="note">2011-11-26</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td><p>With DarkRadiant 1.7.0 a massive list of improvements has been made available, next to the usual long list of bugfixes. A fully-fledged Particle Editor, real-time render preview,
	  increased map loading performance, reduced memory consumption and many improvements related to layers, to name the most important changes over the previous release.</p>
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
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.7.0/darkradiant-1.7.0.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.7.0/darkradiant-1.7.0.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows 32-bit) </li>
          </ul>
          <p class="subheadline">Windows 64-bit</p>
          <ul>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.7.0/darkradiant-1.7.0.x64.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.7.0/darkradiant-1.7.0.x64.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows x64) </li>
          </ul>
          <p class="subheadline">Ubuntu / Kubuntu Linux</p>
          <ul>
            <li>Please follow the instructions on our <a href="https://launchpad.net/~orbweaver/+archive/darkradiant">Launchpad page</a> to download a DarkRadiant package for Ubuntu.</li>
          </ul></td>
    </tr>
  </table>

  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 1.6.1</th>
      <th width="150" class="note">2011-04-23</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td><p>DarkRadiant 1.6.1 is a maintenance or bugfix release which resolves a few issues that came up since 1.6.0.</p>
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
          </ul></td>
    </tr>
  </table>

  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 1.6.0</th>
      <th width="150" class="note">2011-04-08</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td><p>DarkRadiant 1.6.0 introduces native support for the Quake 4 Map Format as well as a rudimentary quake4.game definition (to be tested, feedback is welcome). The 3D renderer went through some profiling and
			is operating considerably faster now.  A few bugs and crashes have been fixed as well.</p>
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
          </ul></td>
    </tr>
  </table>

  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 1.5.0</th>
      <th width="150" class="note">2011-01-21</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td><p>As most prominent feature DarkRadiant 1.5.0 provides a newly written Particle Previewer, including real-time particle rendering. Besides a few bugfixes and usability improvements, the major changes happened behind the scenes (all the UI code has been refactored to use GTK's C++ interface gtkmm).</p>
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
          </ul></td>
    </tr>
  </table>

  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 1.4.0</th>
      <th width="150" class="note">2010-07-21</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td colspan="2"><p>The 1.4.0  release introduces a small set of new features, including Selection Sets, a new Group Part selection mode, Vocal Set  Chooser (for TDM 1.03+) and a couple of bugfixes.</p>
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
        </ul></td>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 1.3.2</th>
      <th width="150" class="note">2010-06-20</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td colspan="2"><p>This is a bugfix release, resolving a couple of issues related to filtering, decal rendering and curve handling.</p>
          <p class="subheadline">Important</p>
        <p>Be sure to install  the <strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en" target="_blank">VC++ 2008</a></strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en"> redistributable package</a> in order to run this release. </p>
        <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
        <p class="subheadline">Windows 32-bit</p>
        <ul>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.3.2/darkradiant-1.3.2.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
          <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.3.2/darkradiant-1.3.2.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows 32-bit) </li>
        </ul>
        <p class="subheadline">Windows 64-bit</p>
        <ul>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.3.2/darkradiant-1.3.2.x64.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
          <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.3.2/darkradiant-1.3.2.x64.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows x64) </li>
        </ul>
        <p class="subheadline">Ubuntu / Kubuntu Linux</p>
        <ul>
            <li>Please follow the instructions on our <a href="https://launchpad.net/~orbweaver/+archive/darkradiant">Launchpad page</a> to download a DarkRadiant package for Ubuntu.</li>
        </ul></td>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 1.3.1</th>
      <th width="150" class="note">2010-05-30</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td colspan="2"><p>This is a bugfix release superseding the recently published 1.3.0 feature release, resolving a few annoying crashes related to the Objectives Editor plug-in. No new features have been introduced, except for the ability to select the camera position in Splitpane layout.</p>
          <p class="subheadline">Important</p>
          <p>Be sure to install  the <strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en" target="_blank">VC++ 2008</a></strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en"> redistributable package</a> in order to run this release. </p>
          <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
          <p class="subheadline">Windows 32-bit</p>
          <ul>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.3.1/darkradiant-1.3.1.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.3.1/darkradiant-1.3.1.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows 32-bit) </li>
          </ul>
          <p class="subheadline">Windows 64-bit</p>
          <ul>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.3.1/darkradiant-1.3.1.x64.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.3.1/darkradiant-1.3.1.x64.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows x64) </li>
          </ul>
          <p class="subheadline">Ubuntu / Kubuntu Linux</p>
          <ul>
            <li>Please follow the instructions on our <a href="https://launchpad.net/~orbweaver/+archive/darkradiant">Launchpad page</a> to download a DarkRadiant package for Ubuntu.</li>
          </ul></td>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 1.3.0</th>
      <th width="150" class="note">2010-05-25</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td colspan="2"><p>This feature release introduces support for multiple languages. German is included as first &quot;foreign&quot; language - if you're interested in translating DarkRadiant into your language, feel free to contact us.</p>
        <p>Apart from internationalization, DarkRadiant 1.3.0 comes with a few bugfixes and usability improvements.</p>
        <p class="subheadline">Important</p>
        <p>Be sure to install  the <strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en" target="_blank">VC++ 2008</a></strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en"> redistributable package</a> in order to run this release. </p>
        <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
        <p class="subheadline">Windows 32-bit</p>
        <ul>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.3.0/darkradiant-1.3.0.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
          <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.3.0/darkradiant-1.3.0.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows 32-bit) </li>
        </ul>
        <p class="subheadline">Windows 64-bit</p>
        <ul>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.3.0/darkradiant-1.3.0.x64.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
          <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.3.0/darkradiant-1.3.0.x64.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows x64) </li>
        </ul>
        <p class="subheadline">Ubuntu / Kubuntu Linux</p>
        <ul>
            <li>Please follow the instructions on our <a href="https://launchpad.net/~orbweaver/+archive/darkradiant">Launchpad page</a> to download a DarkRadiant package for Ubuntu.</li>
        </ul></td>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 1.2.2</th>
      <th width="150" class="note">2010-04-19</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td colspan="2"><p>This is a regular maintenance/bugfix release, resolving some crashes and adding support for automatically disabling Windows desktop composition on startup.</p>
          <p class="subheadline">Important</p>
        <p>Be sure to install  the <strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en" target="_blank">VC++ 2008</a></strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en"> redistributable package</a> in order to run this release. </p>
        <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
        <p class="subheadline">Windows 32-bit</p>
        <ul>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.2.2/darkradiant-1.2.2.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
          <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.2.2/darkradiant-1.2.2.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows 32-bit) </li>
        </ul>
        <p class="subheadline">Windows 64-bit</p>
        <ul>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.2.2/darkradiant-1.2.2.x64.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
          <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.2.2/darkradiant-1.2.2.x64.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows x64) </li>
        </ul>
        </td>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 1.2.1</th>
      <th width="150" class="note">16/03/2010</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td colspan="2"><p>A critical bug surfaced in the recently released 1.2.0 preventing fonts in PK4 files from being recognised by DarkRadiant's readable editor.</p>
          <p class="subheadline">Important</p>
        <p>Be sure to install  the <strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en" target="_blank">VC++ 2008</a></strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en"> redistributable package</a> in order to run this release. </p>
        <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
        <p class="subheadline">Windows 32-bit</p>
        <ul>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.2.1/darkradiant-1.2.1.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
          <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.2.1/darkradiant-1.2.1.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows 32-bit) </li>
        </ul>
        <p class="subheadline">Windows 64-bit</p>
        <ul>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.2.1/darkradiant-1.2.1.x64.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
          <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.2.1/darkradiant-1.2.1.x64.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows x64) </li>
        </ul>
        </td>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 1.2.0</th>
      <th width="150" class="note">12/03/2010</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td colspan="2"><p>The most prominent feature in this release is the newly written <strong>Readable Editor</strong> plugin, making WYSIWYG editing of The Dark Mod readables finally possible.</p>
          <p align="left">Plus a couple of new features and (performance) improvements round up the release of DarkRadiant 1.2.0. </p>
          <p class="subheadline">Important</p>
          <p>Be sure to install  the <strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en" target="_blank">VC++ 2008</a></strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en"> redistributable package</a> in order to run this release. </p>
          <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
          <p class="subheadline">Windows 32-bit</p>
          <ul>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.2.0/darkradiant-1.2.0.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.2.0/darkradiant-1.2.0.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows 32-bit) </li>
          </ul>
          <p class="subheadline">Windows 64-bit</p>
          <ul>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.2.0/darkradiant-1.2.0.x64.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.2.0/darkradiant-1.2.0.x64.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows x64) </li>
          </ul>
          </td>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 1.1.0</th>
      <th width="150" class="note">16/01/2010</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td colspan="2"><p>A <strong>massive</strong> list of improvements made it into this release, I  strongly recommend upgrading to the this newest version. New texturing tools are available,  overall performance has been improved, Python scripting support has been enhanced, and a couple of stability and usability changes made it into this release.</p>
          <p class="subheadline">Important</p>
        <p>Be sure to install  the <strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en" target="_blank">VC++ 2008</a></strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en"> redistributable package</a> in order to run this release. </p>
        <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
        <p class="subheadline">Windows 32-bit</p>
        <ul>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.1.0/darkradiant-1.1.0.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
          <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.1.0/darkradiant-1.1.0.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows 32-bit) </li>
        </ul>
        <p class="subheadline">Windows 64-bit</p>
        <ul>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.1.0/darkradiant-1.1.0.x64.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
          <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.1.0/darkradiant-1.1.0.x64.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows x64) </li>
        </ul>
        </td>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 1.0.2</th>
      <th width="150" class="note">26/10/2009</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td colspan="2"><p>The critical bug surfaced in the recently released 1.0.0 was still not fixed in 1.0.1 hence a new bugfix release was in order.</p>
          <p class="subheadline">Important</p>
        <p>Be sure to install  the <strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en" target="_blank">VC++ 2008</a></strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en"> redistributable package</a> in order to run this release. </p>
        <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
        <p class="subheadline">Windows 32-bit</p>
        <ul>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.0.2/darkradiant-1.0.2.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
          <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.0.2/darkradiant-1.0.2.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows 32-bit) </li>
        </ul>
        <p class="subheadline">Windows 64-bit</p>
        <ul>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.0.2/darkradiant-1.0.2.x64.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
          <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.0.2/darkradiant-1.0.2.x64.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows x64) </li>
        </ul>
        </td>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 1.0.1</th>
      <th width="150" class="note">24/10/2009</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td colspan="2"><p>A critical bug surfaced in the recently released 1.0.0  which crashed the application on cloning patches. This has been fixed, as long with two other minor bugs.</p>
          <p class="subheadline">Important</p>
        <p>Be sure to install  the <strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en" target="_blank">VC++ 2008</a></strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en"> redistributable package</a> in order to run this release. </p>
        <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
        <p class="subheadline">Windows 32-bit</p>
        <ul>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.0.1/darkradiant-1.0.1.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
          <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.0.1/darkradiant-1.0.1.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows 32-bit) </li>
        </ul>
        <p class="subheadline">Windows 64-bit</p>
        <ul>
          <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.0.1/darkradiant-1.0.1.x64.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
          <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.0.1/darkradiant-1.0.1.x64.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows x64) </li>
        </ul>
      </td>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 1.0.0</th>
      <th width="150" class="note">16/10/2009</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td colspan="2"><p>After three years of development DarkRadiant 1.0.0 finally sees the light of day. </p>
        <p>Although this new release is mainly a &quot;stabilising&quot; one including lots of bugfixes, the version bump to 1.0.0 is accompanying the release of DarkRadiant's &quot;sister project&quot; <a href="http://www.thedarkmod.com/" target="_blank">The Dark Mod</a> 1.00. We think that the editor is mature enough in the meantime to justify the sudden version increase.</p>
        <p>This release supercedes the previous one, as usual. </p>
        <p class="subheadline">Important</p>
        <p>Be sure to install  the <strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en" target="_blank">VC++ 2008</a></strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en"> redistributable package</a> in order to run this release. </p>
        <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
        <p class="subheadline">Windows 32-bit</p>
        <ul>
            <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.0.0/darkradiant-1.0.0.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
          <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.0.0/darkradiant-1.0.0.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows 32-bit) </li>
        </ul>
        <p class="subheadline">Windows 64-bit</p>
        <ul>
          <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.0.0/darkradiant-1.0.0.x64.exe/download" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
          <li><a href="https://sourceforge.net/projects/darkradiant/files/darkradiant/1.0.0/darkradiant-1.0.0.x64.zip/download" target="_blank"><strong>Download</strong></a> (ZIP, Windows x64) </li>
        </ul>
      </td>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 0.10.0</th>
      <th width="150" class="note">21/06/2009</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td colspan="2"><p>DarkRadiant 0.10.0 includes an upgraded render and shader system, to improve support for id tech 4 materials and to give a better preview of maps in lighting mode. This point release also resolves some problems observed on multi-monitor setups.</p>
          <p>New features include support for 3D-rotatable entities like func_emitters and light entities showing their models when the corresponding property is set. It's now possible to resize the speaker radius by mouse drags and to let the entity origin untouched during these operations (also applies to light resize operations).</p>
          <p> This supercedes the previous release, as usual. </p>
          <p class="subheadline">Important</p>
        <p>Be sure to install  the <strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en" target="_blank">VC++ 2008</a></strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en"> redistributable package</a> in order to run this release. </p>
        <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
        <p class="subheadline">Windows 32-bit</p>
        <ul>
          <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.10.0.exe" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
          <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.10.0.zip" target="_blank"><strong>Download</strong></a> (ZIP, Windows 32-bit) </li>
        </ul>
        <p class="subheadline">Windows 64-bit</p>
        <ul>
          <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.10.0.x64.exe" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
          <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.10.0.x64.zip" target="_blank"><strong>Download</strong></a> (ZIP, Windows x64) </li>
        </ul>
        </td>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 0.9.12</th>
      <th width="150" class="note">12/03/2009</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td colspan="2"><p>This is a bugfix release addressing a bug in the shader file parser. Many models using shaders without qer_editorimage expressions were showing up with &quot;shader not found&quot;. This supercedes the previous release, as usual. </p>
          <p class="subheadline">Important</p>
        <p>Be sure to install  the <strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en" target="_blank">VC++ 2008</a></strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en"> redistributable package</a> in order to run this release. </p>
        <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
        <p class="subheadline">Windows 32-bit</p>
        <ul>
            <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.12.exe" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
          <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.12.zip" target="_blank"><strong>Download</strong></a> (ZIP, Windows 32-bit) </li>
        </ul>
        <p class="subheadline">Windows 64-bit</p>
        <ul>
            <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.12.x64.exe" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
          <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.12.x64.zip" target="_blank"><strong>Download</strong></a> (ZIP, Windows x64) </li>
        </ul>
        </td>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 0.9.11</th>
      <th width="150" class="note">09/03/2009</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td colspan="2"><p>This release   features a newly written command system under the hood - DarkRadiant has its own command console now, making it possible to fire operations by typing and to create new command aliases and &quot;binds&quot;. </p>
          <p>As another major feature, a new scripting plugin is included in this release, introducing an interface for Python scripts. Scripts can be used now to add even more algorithms to DarkRadiant without recompiling the source. The work on the scripting documentation is kind of work in progress, expect some tutorials to be posted on our wiki in the near future. </p>
          <p>These features, and numerous bug fixes round up the list of changes for this new package.</p>
          <p class="subheadline">Important</p>
          <p>Be sure to install  the <strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en" target="_blank">VC++ 2008</a></strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en"> redistributable package</a> in order to run this release. </p>
          <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
          <p class="subheadline">32-bit</p>
          <ul>
            <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.11.exe" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
            <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.11.zip" target="_blank"><strong>Download</strong></a> (ZIP, Windows 32-bit) </li>
          </ul>
          <p class="subheadline">64-bit</p>
          <ul>
            <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.11.x64.exe" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
            <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.11.x64.zip" target="_blank"><strong>Download</strong></a> (ZIP, Windows x64) </li>
          </ul></td>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 0.9.10</th>
      <th width="150" class="note">06/02/2009</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td colspan="2"><p>Development on the editor has made quite some strides in the past month, and DarkRadiant 0.9.10 is ready for release. There have been a few bugfixes, many usability improvements and better DEF file parsing support as well as a newprefab preview window. </p>
          <p class="subheadline">Important</p>
        <p>Be sure to install  the <strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en" target="_blank">VC++ 2008</a></strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en"> redistributable package</a> in order to run this release.</p>
        <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
        <p class="subheadline">32-bit</p>
        <ul>
          <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.10.exe" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
          <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.10.zip" target="_blank"><strong>Download</strong></a> (ZIP, Windows 32-bit) </li>
        </ul>
        <p class="subheadline">64-bit</p>
        <ul>
          <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.10.x64.exe" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
          <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.10.x64.zip" target="_blank"><strong>Download</strong></a> (ZIP, Windows x64) </li>
        </ul></td>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 0.9.9</th>
      <th width="150" class="note">30/12/2008</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td colspan="2"><p>Development on the editor has been progressing nicely in December. DarkRadiant 0.9.9 includes a lot of noticeable improvements, including improved DDS texture handling, better memory consumption, new GUIs and lots of bugfixes and usability changes. This release is also the first one including a build targetting the Windows x64 platform (Vista 64). </p>
          <p class="subheadline">Important</p>
        <p>Be sure to install  the <strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en" target="_blank">VC++ 2008</a></strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en"> redistributable package</a> in order to run this release.</p>
        <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
        <p class="subheadline">32-bit</p>
        <ul>
          <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.9.1.exe" target="_blank"><strong>Download</strong></a> (Installer, Windows 32-bit)</li>
          <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.9.1.zip" target="_blank"><strong>Download</strong></a> (ZIP, Windows 32-bit) </li>
        </ul>
        <p class="subheadline">64-bit</p>
        <ul>
          <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.9.1.x64.exe" target="_blank"><strong>Download</strong></a> (Installer, Windows x64)</li>
          <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.9.1.x64.zip" target="_blank"><strong>Download</strong></a> (ZIP, Windows x64) </li>
        </ul></td>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 0.9.8</th>
      <th width="150" class="note">07/12/2008</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td colspan="2"><p>Development on the editor has been steadily progressing and DarkRadiant 0.9.8 is ready for release. It contains tons of fixes and a new Conversation Editor GUI  to facilitate editing dialogs in DarkMod maps.</p>
        <p class="subheadline">Important</p>
        <p>Be sure to install  the <strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en" target="_blank">VC++ 2008</a></strong><a href="http://www.microsoft.com/downloads/details.aspx?FamilyID=9B2DA534-3E03-4391-8A4D-074B9F2BC1BF&amp;displaylang=en"> redistributable package</a> in order to run this release.</p>
        <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
        <ul>
            <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.8.1.exe" target="_blank"><strong>Download</strong></a> (Installer)</li>
          <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.8.1.zip" target="_blank"><strong>Download</strong></a> (ZIP)</li>
        </ul></td>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 0.9.7</th>
      <th width="150" class="note">29/08/2008</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td colspan="2"><p>After a couple of months of development DarkRadiant 0.9.7 is ready for a public release. It contains a number of bugfixes, a rewritten namespace and a new Objectives GUI  to facilitate editing objectives in DarkMod maps.</p>
          <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/ChangeLog?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
        <ul>
            <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.7.exe" target="_blank"><strong>Download</strong></a> (Installer)</li>
            <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.7.zip" target="_blank"><strong>Download</strong></a> (ZIP) </li>
            <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant_0.9.7_i386.deb" target="_blank"><strong>Download</strong></a> (DEB) </li>
        </ul></td>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 0.9.6</th>
      <th width="150" class="note">06/04/2008</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td colspan="2"><p>After three months of intensive development DarkRadiant 0.9.6 is ready for a public release. It contains a number of bugfixes, support for layers and a Difficulty Editor GUI specifically for editing DarkMod-maps. </p>
        <p>As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/CHANGES?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
        <ul>
            <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.6.exe" target="_blank"><strong>Download</strong></a> (Installer)</li>
            <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.6.zip" target="_blank"><strong>Download</strong></a> (ZIP) </li>
            <li><strong><a href="http://downloads.sourceforge.net/darkradiant/darkradiant_0.9.6_i386.deb" target="_blank">Download</a></strong> (DEB) </li>
        </ul></td>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 0.9.5</th>
      <th width="150" class="note">19/01/2008</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
    <tr>
      <td colspan="2"><p>It was a rather long time since the last release, but finally DarkRadiant 0.9.5 has arrived. It further improves the support for MD5 models and skins. A new plug-in has been developed to allow issuing &quot;dmap&quot; commands to a running TDM instance. Bugs have been fixed, things have been tweaked.  As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/CHANGES?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
          <ul>
            <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.5.exe" target="_blank"><strong>Download</strong></a> (Installer)</li>
            <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.5.zip" target="_blank"><strong>Download</strong></a> (ZIP) </li>
          </ul></td>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="header">
    <tr>
      <th>DarkRadiant 0.9.4</th>
      <th width="150" class="note">02/11/2007</th>
    </tr>
  </table>
  <table cellspacing="0" cellpadding="0" class="content">
      <tr>
        <td colspan="2"><p>This is a bugfix release addressing an issue with the inheritance of  entity classes in the Entity Browser, with a couple of other tweaks.  As usual, you can also take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/CHANGES?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
            <ul>
              <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.4.exe" target="_blank"><strong>Download</strong></a> (Installer)</li>
              <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.4.7z" target="_blank"><strong>Download</strong></a> (7-Zip)</li>
            </ul></td>
      </tr>
  </table>
<table cellspacing="0" cellpadding="0" class="header">
      <tr>
        <th>DarkRadiant 0.9.3</th>
        <th width="150" class="note">21/10/2007</th>
      </tr>
    </table>
	<table cellspacing="0" cellpadding="0" class="content">
      <tr>
        <td colspan="2"><p>This is a minor release with a couple of bugfixes and tweaks, and is  also the first release which contains the refactored module system  (which should make no visible difference to the user unless there is  some bug which we haven't found).</p>
            <p>Check out the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/CHANGES?view=markup" target="_blank">developer changelog</a>, if you're interested in a more detailed list.</p>
            <ul>
              <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.3.exe" target="_blank"><strong>Download</strong></a> (Installer)</li>
            <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.3.7z" target="_blank"><strong>Download</strong></a> (7-Zip)</li>
          </ul></td>
      </tr>
    </table>
	<table cellspacing="0" cellpadding="0" class="header">
      <tr>
        <th>DarkRadiant 0.9.2</th>
        <th width="150" class="note">06/09/2007</th>
      </tr>
    </table>
	<table cellspacing="0" cellpadding="0" class="content">
      <tr>
        <td colspan="2"><p>This release adds support of CurveNURBS and CurveCatmullROM control vertex editing, better Doom 3 shader support (<em>addnormals</em> and other MapExpressions, built-in textures like <em>_white</em>, etc.), a mod-based grouping of the elements in the Entity Chooser and many other bugfixes, tweaks, usability and performance improvements.</p>
            <p>Check out the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/CHANGES?view=markup" target="_blank">developer changelog</a>, if you're interested in a more detailed list.</p>
            <ul>
              <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.2.exe" target="_blank"><strong>Download</strong></a> (Installer)</li>
            <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.2.7z" target="_blank"><strong>Download</strong></a> (7-Zip)</li>
          </ul></td>
      </tr>
    </table>
	<table cellspacing="0" cellpadding="0" class="header">
      <tr>
        <th>DarkRadiant 0.9.1</th>
        <th width="150" class="note">10/06/2007</th>
      </tr>
    </table>
	<table cellspacing="0" cellpadding="0" class="content">
      <tr>
        <td colspan="2"><p>New in this release: SoundShader playback, improved handling of func_* entities, draggable func_* origin, <em>Add/Move Player Start here</em> option in context menu, fixed and improved patch vertex commands (Add/Delete/Append patch columns/rows) and a new <em>Select Children</em> command. </p>
          <p>Check out the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/CHANGES?view=markup" target="_blank">developer changelog</a>, if you're interested in a more detailed list.</p>
          <ul>
            <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.1.exe" target="_blank"><strong>Download</strong></a> (Installer)</li>
              <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.1.7z" target="_blank"><strong>Download</strong></a> (7-Zip)</li>
          </ul></td>
      </tr>
    </table>
	<table cellspacing="0" cellpadding="0" class="header">
      <tr>
        <th>DarkRadiant 0.9.0</th>
        <th width="150" class="note">29/04/2007</th>
      </tr>
    </table>
	<table cellspacing="0" cellpadding="0" class="content">
      <tr>
        <td colspan="2"><p>This release contains a massive amount of improvements. Take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/CHANGES?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
            <ul>
              <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.0.exe" target="_blank"><strong>Download</strong></a> (Installer)</li>
              <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.9.0.7z" target="_blank"><strong>Download</strong></a> (7-Zip)</li>
            </ul></td>
      </tr>
    </table>
	<table cellspacing="0" cellpadding="0" class="header">
		<tr>
			<th>DarkRadiant 0.8.1</th>
			<th width="150" class="note">28/01/2007</th>
		</tr>
	</table>
	<table cellspacing="0" cellpadding="0" class="content">
		<tr>
			<td colspan="2"><p>This release fixes a few major bugs discovered in the previous release. Take a look at the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/CHANGES?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes.</p>
			<ul><li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.8.1.exe" target="_blank"><strong>Download</strong></a> (Installer)</li>
			  <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.8.1.zip" target="_blank"><strong>Download</strong></a> (ZIP)</li>
	          </ul>
		    </td>
	  </tr>
	</table>
	<table cellspacing="0" cellpadding="0" class="header">
		<tr>
			<th>DarkRadiant 0.8.0</th>
			<th width="150" class="note">26/01/2007</th>
		</tr>
	</table>
	<table cellspacing="0" cellpadding="0" class="content">
		<tr>
			<td colspan="2"><p>A couple of new features made it into this release, like a new LightInspector and the support for projected lights. New texturing tools and a skin chooser are available among other things. View the <a href="http://darkradiant.svn.sourceforge.net/viewvc/darkradiant/trunk/darkradiant/CHANGES?view=markup" target="_blank">developer changelog</a>, if you're interested in a detailed list of changes or take a look.</p>
			  <ul>
			    <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.8.0.exe" target="_blank"><strong>Download</strong></a> (Installer)</li>
			  <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.8.0.zip" target="_blank"><strong>Download</strong></a> (ZIP)</li>
	          </ul>
		    </td>
	  </tr>
	</table>
	<table cellspacing="0" cellpadding="0" class="header">
		<tr>
			<th>DarkRadiant 0.7.1</th>
			<th width="150" class="note">26/11/2006</th>
		</tr>
	</table>
	<table cellspacing="0" cellpadding="0" class="content">
		<tr>
			<td colspan="2"><p>Contains an improved Filter System, a new Media Browser, customisable colour schemes and numerous improvements over the previous release. </p>
			  <ul>
			    <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.7.1.exe" target="_blank"><strong>Download</strong></a> (Installer)</li>
			  <li><a href="http://downloads.sourceforge.net/darkradiant/darkradiant-0.7.1.7z" target="_blank"><strong>Download</strong></a> (7-ZIP)</li>
	          </ul>
		    </td>
	  </tr>
	</table>
