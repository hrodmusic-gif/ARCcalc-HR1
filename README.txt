ARCcalc HR1
v5.6 Portrait Fill PWA

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
