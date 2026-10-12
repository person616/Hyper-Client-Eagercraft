# Hyper Client website

`index.html` and `Hyper-Client.html` are each complete, standalone copies of the game and Hyper Client overlay. The default site address (`/`) uses `index.html`; to use the named file, open `/Hyper-Client.html` instead.

## Fastest options (all free)
**Netlify Drop** – go to app.netlify.com/drop and drag this whole folder in. Done, you get a link.
**GitHub Pages** – make a repo, upload the website folder, then Settings > Pages > Deploy from branch (main, / root).
**Cloudflare Pages** – Workers & Pages > Create > Pages > Upload assets, drop the folder.

Must be served over HTTPS (all of the above are).
Press **Right Shift** in-game for the Hyper Client menu. Change this shortcut in **Style → Controls**.

Startup shows the Hyper Client loading screen over the game's loader. The ⚡ MODS button is created immediately when the page starts, above the loading screen, and stays visible while the panel is open or closed and during gameplay. Game audio stays muted until the loading screen is dismissed. It fades automatically when the main menu is detected; a **Start game** button appears when Edit Profile is detected or after 10 seconds if detection does not trigger. Toggle **Hyper Client loading screen** in the Mods tab to turn it off for future launches.

In **Mods**, click a mod's name to expand its animated settings; its switch independently enables or disables it. HUD mods offer display options. Enable **Toggle Sprint** or **Toggle Sneak** in **Gameplay**, then set each mod's key to the matching key in Minecraft's **Controls** menu; tap that key while playing to toggle the action. For Zoomify-style zoom, hold the configured key while playing and scroll up to zoom in or down to zoom out (1.25×–5×); the panel also lets you choose the starting magnification and key. This zoom is a browser-side approximation, not a port of the Fabric mod. The FPS/frame-time HUD is a simple browser-side equivalent of a mod in the supplied pack. Use **EDIT** in the panel header to move the HUD and keystrokes overlay; dragging is disabled outside edit mode. Choose **DONE** to return to normal play. Closing the panel also exits edit mode.

On the main menu, the original game wordmark is covered by a Hyper Client brand mark styled after the loading-screen **H** tile, with the full **HYPER CLIENT** name. The Hyper Client **⚡ MODS** button stays at the configured screen position (top-right by default) at all times, including while the panel is open or gameplay has pointer lock. Open the button to access the panel; the game's original buttons remain unchanged.

The logo is detected from the three-button main-menu layout, with an adaptive scan for different canvas sizes. Similar dialogs with three stacked blue buttons may also match. The Mods button does not depend on menu detection. For a clean redeploy of this branding fix, upload the entire `Hyper Client Website 1.0 Main` folder to Netlify Drop. The included `_headers` file disables browser caching so the latest uploaded page is fetched.

Open the **Perf** tab to change render resolution (50%, 75%, 100%, or Native). New settings default to 75%; reload the page after changing resolution. HUD and background-pause toggles start off for new settings and can be enabled in the panel.

Hyper Client settings and the Eaglercraft profile (username, skin, and cape) are saved in this browser's local storage. They stay on this device and browser profile; they are not looked up by IP or synced to other devices. Clearing site/browser data or opening a separately hosted copy can use a different storage location.
