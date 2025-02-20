This document is the authoritative source for TurboWarp's changelogs. Everything else gets generated from this list.

Prefix notes with "Windows:", "macOS:", or "Linux:" as needed. Do not use **formatting** or [links](https://desktop.turbowarp.org/).

# 1.9.0-beta.6 (2023-08-25)

 - Fixed mouse inputs.

# 1.9.0-beta.4 (2023-08-25)

 - Desktop app was rewritten for improved security
 - Added custom reporters
 - Added custom fonts
 - New extensions: HTTP, Cast, NFCWarp, Clipboard, Zip, More Motion, LZ String, Longman Dictionary, Skins, All Menus, Custom Styles, Deltatime, Wake Lock
 - Brand new restore point system that is much more reliable than the old one. Now stores multiple restore points and the interval can be customized
 - The builtin costume, sound, sprite, and extension libraries now let you mark items as favorites so they show up first
 - Extension gallery is no longer a separate window, rather it is built in to the editor
 - Improved file saving error handling
 - Fixed backpacking scripts and sprites that contain custom extensions
 - Allow importing .ogg, .flac, and .aac audio files
 - Updated prompt modal
 - Removed "for each" block from the palette because it causes various issues
 - Fixed a lot of bugs

# 1.8.1 (2023-06-20)

 - Fixed issues using custom extensions in the packager (if issues remain, press "Reset All Settings" in packager)
 - Fixed using an extension to fetch files from extensions.turbowarp.org in the editor
 - Fixed Looks Plus "this sprite" option not working properly in clones

# 1.8.0 (2023-06-19)

 - Added more than 40 new extensions including Animated Text (like Scratch Lab), Local Storage, BigInt, JSON, Clipping and Blending, Sensing Plus, Clones Plus, Looks Plus, and RegExp
 - Updated many extensions including Stretch, Runtime Options, and Files
 - To protect user privacy, builtin extensions now ask for permission before allowing the project to contact untrusted websites
 - Custom extensions can now be loaded from files or text
 - Added option to allow extensions to bypass CORS
 - Added "random direction" option to point towards block
 - Fixed script execution order occasionally changing after saving project
 - Fixed zooming with ctrl+plus on some keyboard layouts
 - Fixed exporting addon settings
 - Fixed many other bugs
 - Windows: Support for Windows 7, 8, and 8.1 will be removed in a future release
 - Windows: Added native support for Windows on ARM

# 1.7.1 (2023-01-24)

 - Added support for unsandboxed extensions from extensions.turbowarp.org
 - The desktop app includes an offline copy of extensions.turbowarp.org
 - Custom extensions will now be automatically loaded when you open a project made with recent versions of TurboWarp (a confirmation prompt appears for third-party extensions)
 - Project saving now uses significantly less memory
 - The old button to open the packager in the "?" menu has been moved; use the button in the "File" menu instead. The old button has mentioned the new location for a while. This matches the web app.
 - Added "Rename broadcasts" addon (enabled by default)
 - Added "Collapsing sprite properties" addon
 - Added "Costume editor snapping" addon
 - Added "Project volume slider" addon
 - Added "Always show number pad" addon
 - Added a few more switches to the "Block switching" addon
 - Checkboxes in the toolbox are now dark in dark mode
 - Allow creating monitors for mouse down, mouse x, mouse y, and days since 2000
 - Fixed crash in costume editor using transparent colors with bitmap line tool
 - Fixed costume editor color picker ignoring transparency
 - Fixed some keyboard shortcuts not working when caps lock is enabled
 - Fixed many other bugs
 - Windows: Support for Windows 7, Windows 8, and Windows 8.1 may be removed in a future update
 - macOS: Our app is now notarized by Apple

# 1.6.1 (2022-10-07)

 - Fixed features that access your microphone or camera
 - Fixed addon settings import not importing some color options

# 1.6.0 (2022-10-02)

 - New addon: Pick colors from stage (enabled by default)
 - New addon: Zebra striping
 - Bitmap costume editor now supports transparency
 - SVGs exported by TurboWarp and imported to TurboWarp won't be re-centered unnecessarily
 - Sound editor now shows a sound's size, whether it's stereo or not, and its sample rate
 - Maximum SVG size has been reverted to the same as Scratch due to too many crashes
 - Added option to clone counter to only show icon
 - Added "Turbo Robot" sprite to builtin libraries
 - Added option to customizable new sprite position to apply to duplicated sprites
 - Fixed "Saving project..." text disappearing before the project was actually saved
 - Fixed save location still being updated if you cancel the confirmation to replace existing project
 - Fixed unnecessary memory use when saving files
 - Fixed loading some projects with many bitmap costumes
 - Fixed block cherry picking breaking on certain blocks
 - Fixed tangent block reporting slightly incorrect values in the compiler
 - Fixed display stage on left side and two-column category menu compatibility bugs
 - Fixed developer tools dark mode issue
 - Fixed auto-hiding block palette bugs
 - Fixed variable manager bugs
 - Fixed sound editor layout bugs at certain window sizes
 - Fixed some costume and sound lists having an unnecessary horizontal scrollbar
 - Fixed color picker overlay not covering the entire page
 - Fixed some icons being unnecessarily draggable
 - Fixed loading Scratch 2 projects with unusual JSON
 - Windows: Title bar now respects your computer's dark mode preference
 - Linux: We now have a repository for Debian/Ubuntu and their derivatives
 - Updated packager: settings export and import, optimized memory use of packaged projects

# 1.5.0 (2022-07-23)

 - New addon: Reverse order of project controls
 - New addon: Hide stage and sprite pane
 - Allow creating unlimited cloud variables
 - Fixed backpacking JPEG costumes
 - Fixed turbo mode stored in projects not applying properly
 - Added option to disable hidden window throttling
 - Fixed some bugs in the auto-hiding block palette addon
 - Linux: Support for 32-bit x86 has been removed
 - macOS: Fixed uncloseable packager windows if opened from a fullscreen editor window
 - Updated packager: list color, version number, macOS Electron, Scratch Link support, more

# 1.4.0 (2022-06-24)

 - Moved the builtin copy of the TurboWarp Packager to the File > Package project menu
 - Added a sound duration indicator to the sound editor
 - Added partial support for the "Threads" tab in the debugger addon, including single stepping
 - Fixed high CPU usage when project is paused
 - Increased maximum resolution of large vector costumes
 - Updated backpacked item previews to support transparency
 - Updated dark mode with improved inputs, improved scrollbars, and support for the debugger and gamepad addons
 - Fixed developer tools find bar covering up controls in certain conditions
 - Fixed variable manager causing crashes when variables are too large
 - Improved style of many modals and prompts to be more cohesive
 - Fixed block context menus immediately selecting item and closing after being opened on some systems
 - Fixed interface allowing invalid framerates and invalid stage sizes
 - Fixed custom extensions being able to corrupt projects if they return unexpected values
 - Fixed custom extension error handling
 - Fixed various other bugs
 - Linux: Support for 32-bit x86 systems will be removed in v1.5.0 (32-bit ARM is not affected)
 - Linux: Added support for Linux on Apple Silicon
 - macOS: Reduced app startup time
 - Added donation links
 - Updated packager: adds support for "☁ room id" special cloud behavior

# 1.3.1 (2022-05-18)

 - Fixed crash on some Linux systems
 - Gamepad addon now supports buttons other than the left button and is compatible with pointerlock in the packager
 - Updated packager: relicensed to Apache 2.0 from LGPL3.0 for fewer restrictions, added "☁ set clipboard" and "☁ pasted" support to special cloud behaviors
 - Various other bug fixes

# 1.3.0 (2022-05-03)

 - New addon: Customizable default costume editor colors
 - The app now registers itself as a file handler for .sb and sb2 files in addition to .sb3
 - Optimized comparison blocks
 - Fixed more crashes on app startup on some systems

# 1.2.2 (2022-04-13)

 - Fixed mouse actions in gamepad support addon in packager
 - Fixed blocks like "insert x at any of list" to insert at a random location

# 1.2.1 (2022-04-10)

 - Fixed crash on startup on some systems
 - All windows now have proper language hints, fixes CJK characters looking weird in some windows
 - Added error message when any child process dies unexpectedly, not just renderer processes

# 1.2.0 (2022-04-09)

 - Added option to configure which microphone and camera the app should use
 - Added option to disable hardware acceleration
 - Fixed stage size stored in projects
 - Reduced costume editor flicker when switching costumes
 - Added text inputs to costume editor color components
 - Fixed monitor position after resizing stage
 - Fixed vertical centering of variable monitor values in certain conditions
 - Fixed lines between tiled stamps when high quality pen is enabled
 - Reduced lag related to folders addon

# 1.1.3 (2022-2-21)

 - Fixed "Mouse position" addon

# 1.1.2 (2022-02-20)

 - Fixed automatically loading project in packager
 - Fixed significant lag when displaying variable monitors caused by the "Hide new variables" addon
 - Fixed builtin sound library not working when offline or in certain regions of the world (China)
 - "Remove Miscellaneous Limits" now also disables mouse X and Y coordinate rounding

# 1.1.1 (2022-2-13)

 - New addon: Customizable block text style
 - New addon: Search sprites by name
 - New addon: Enhanced full screen
 - The right-click menu on a variable monitor now has an option to hide it
 - Stage size can now be changed without reloading the editor
 - Stage size can now be stored in a project
 - Fix storing gamepad settings in projects
 - Fix onion skinning layers being slightly misplaced
 - Improve sound editor performance on very large sounds
 - Updated packager
 - Many bug fixes

# 1.0.0 (2022-1-15)

 - The costume editor now supports dark mode
 - If a dark background makes it hard to edit your costumes, it's possible to change the theme of the costume editor without effecting the rest of the interface
 - Significantly optimized memory use of costumes
 - Improved project exporting to compress project.json by up to to 30%
 - Many compiler optimizations and compatibility fixes
 - When you right click on a misspelled word detected by the spellchecker, you will now see some suggested replacements
 - Updated integrated packager
 - Various bug fixes
 - Updated translations
