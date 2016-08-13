=== Customizer Dev Tools ===
Contributors:      xwp, westonruter
Tags:              customizer, customize, dev-tools, debug, debugging, developer, development
Requires at least: 4.5
Tested up to:      4.6
Stable tag:        0.7.0
License:           GPLv2 or later
License URI:       http://www.gnu.org/licenses/gpl-2.0.html

Tools for facilitating JavaScript development in the customizer.

== Description ==

Features:

* The `wp.customize` object from the Customizer preview is made persistently available from the parent frame via `CustomizerDevTools.previewCustomize`. This reference is updated whenever the preview refreshes, so you no longer have to change the frame window context to access this object.
* In the same way, the current Customizer preview `window` is exposed as `CustomizerDevTools.previewWindow`.  This is a shortcut for doing `wp.customize.previewer.targetWindow.get()`, and it has the added benefit of allowing the browser's dev tools to provide auto-completion.