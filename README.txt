ARCcalc HR1
v5.16 Beta PWA

Open index.html in a browser for a local preview. For installable/offline PWA behavior, serve this folder over HTTPS or localhost.

Included improvements:
- Bottom tool tabs now sit directly against the bottom of the calculator
- The keypad stretches vertically to use the recovered space
- iPhone safe-area space is carried inside the tab bar instead of appearing as a blank strip
- Portrait-primary PWA orientation remains enabled
- Best-effort portrait orientation lock remains enabled in installed standalone mode
- Removed the landscape warning screen
- Removed the alternate two-column landscape calculator layout from normal use
- A regular browser tab that rotates simply keeps the same portrait canvas
- Desktop and tablet fit-to-window portrait presentation retained
- All v5.1 stability and v5.2 responsive improvements retained


v5.6 DISPLAY NOTE
- Mobile layout no longer follows visualViewport height, preventing iPhone browser chrome from shrinking the calculator.
- The installed PWA requests fullscreen with standalone fallback and remains portrait-only.
- iPhone users should add the hosted PWA to the Home Screen for the closest native-app presentation.


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


## v5.12 native bottom bar
- Reduced the unused space below the bottom tabs on iPhone Home Screen installs.
- Lowered and vertically centered the three tab controls inside the navigation surface.
- Retained enough clearance for the iPhone Home indicator without reserving the entire safe area as blank space.
- Returned the reclaimed height to all eight keypad rows.
- Kept the v5.10/v5.11 full-screen standalone viewport correction.


## v5.13 unified top surface
- Matched the HTML theme color, PWA theme color, startup background, and phone canvas to #222b38.
- Replaced the diagonal phone background at the top edge with a vertically blended surface whose first color is uniform across the full width.
- Removed the one-pixel calculator case outline at the installed-app top edge.
- Preserved the approved v5.12 bottom navigation dimensions and full-height keypad.


## v5.14 Dynamic Island fit
- Moved the brand/header 20 CSS pixels upward on installed modern iPhones.
- Keeps a conservative gap below the Dynamic Island rather than using the entire safe-area inset as empty spacing.
- Returns the recovered height to the keypad automatically.
- Preserves the approved v5.12/v5.13 bottom navigation dimensions and unified top color.


## v5.15 Logo clearance
- Reduced the modern-iPhone header lift from 20px to 10px so the full blue arc remains visible.
- Fixed the logo wrapper at 82px on tall installed iPhones to prevent internal clipping.
- Allows the brand and logo wrapper to overflow visibly while keeping the app viewport clipped.
- Preserves the approved bottom navigation, key sizing, full-screen layout, and unified top color.


## v5.16 Beta
- Removed the legacy top frame highlight that appeared as a divider below the iPhone status bar.
- Settings now shows only “v5.16 Beta” under App version.
- Logo placement, stretched keypad, and approved bottom bar remain unchanged.
