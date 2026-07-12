# ARCcalc HR1 v5.6 Maintenance Notes

## Bottom-fill layout work completed in v5.6

- Converted the final calculator presentation to a four-row grid: branding, display, flexible keypad, and bottom tabs.
- Removed the oversized bottom padding below the tool tabs.
- Made all eight keypad rows share the available height evenly.
- Moved phone safe-area padding into the tool-tab bar so its background reaches the physical bottom edge.
- Removed the mobile landscape warning overlay and its markup.
- Disabled the alternate two-column landscape calculator presentation.
- Kept a fixed portrait canvas if an ordinary mobile browser rotates despite the portrait request.
- Retained `portrait-primary` in the manifest and best-effort Screen Orientation API locking in installed mode.
- Bumped the offline cache to `arccalc-hr1-v5-4-portrait-fill`.

## Retained work

- v5.1 math/runtime stability repairs.
- v5.2 responsive safe-area, visual-viewport, and tool-screen work.
- v5.3 desktop background and portrait-stage fixes.

## Platform limitation

Safari and Chrome do not guarantee orientation locking for a normal browser tab. Orientation locking is requested for the installed PWA. In a normal tab, ARCcalc no longer shows a landscape message or alternate layout; it preserves the portrait canvas.


## v5.6 edge-to-edge presentation
- Removed visualViewport-driven phone height sizing.
- Added largest-viewport browser sizing and full-screen PWA display override.
- Added iOS fill-available/viewport-safe styling and seamless system-area background.
- Added best-effort first-tap fullscreen on supported Android/mobile browsers.


## v5.6 true fullscreen fit
- Removed the duplicated iPhone top safe-area padding.
- Browser previews now size to the actual visible viewport instead of screen.height.
- Installed PWA mode alone applies notch and home-indicator safe areas.
- The tab surface occupies the final grid row and reaches the viewport bottom.


## v5.7 full-height keys
- Mobile portrait now uses the full layout viewport when the keyboard is closed.
- 100lvh provides a fallback for iPhone browser chrome changes.
- All surplus vertical space is distributed across the eight keypad rows.
- Brand, display, and bottom-tab heights remain unchanged.


## v5.8 Home Screen fit
- Installed iPhone/Home Screen mode now uses the exact live app viewport.
- 100lvh is no longer allowed to enlarge an installed app beyond its visible area.
- The stretched eight-row keypad remains, but all tabs stay fully visible.
- Portrait-only behavior is preserved.


## v5.9 iPhone standalone fill
- Corrected the v5.8 black strip caused by using visualViewport.height as document height.
- Installed/Home Screen mode now fills the layout viewport with fixed inset geometry.
- visualViewport is used only to detect an on-screen keyboard.
- Extra height continues to be distributed through the eight keypad rows.
- Bottom tabs and safe-area padding remain fully visible.


## v5.10 iPhone full-screen correction
- Replaced 100dvh with 100vh only in installed/Home Screen mode.
- This restores the top safe-area height that iOS was subtracting and removes the bottom strip.
- Kept 100dvh/visual viewport sizing for ordinary mobile browser tabs.
- Removed fullscreen from display_override; iOS uses the supported standalone mode.
- The HTML canvas and tab bar now share the same bottom surface color.
- Extra height is distributed evenly through all eight keypad rows.


## v5.11 stretched-key layout
- Reduced the visible bottom navigation controls to a compact 36px height.
- The navigation background still covers the iPhone Home-indicator safe area.
- Removed safe-area padding from inside each tab button so the active pill is no longer oversized.
- Redistributed all reclaimed vertical space evenly across the eight keypad rows.
- Retained the v5.10 full-screen Home Screen viewport correction.
