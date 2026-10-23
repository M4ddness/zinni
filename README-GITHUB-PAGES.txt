ZINNI — GITHUB PAGES UPDATE / CACHE FIX

IMPORTANT: Upload BOTH index.html and sw.js from this package. The updated service worker uses a new cache version (zinni-pwa-v3), removes old Zinni caches, claims open tabs, and checks the network first for page navigations so GitHub Pages updates are not hidden by stale cached HTML.

UPDATE AN EXISTING GITHUB PAGES SITE
1. Download and unzip this package.
2. Open your existing Zinni repository on GitHub.
3. At the repository root, choose Add file > Upload files.
4. Upload the NEW index.html and NEW sw.js from this folder. If GitHub asks, confirm that you want to replace the existing files.
5. Click Commit changes.
6. Wait for GitHub Pages to finish deploying (usually a minute or two). Check repository Settings > Pages for deployment status.
7. Open your site in a normal browser tab, then do a hard refresh:
   - Chrome/Edge on Windows: Ctrl + Shift + R
   - Chrome/Edge on Mac: Cmd + Shift + R
   - Safari on Mac: Option + Cmd + R (or clear website data if needed)
8. If the installed app still shows the old version, fully close the installed Zinni window, open the website URL in the browser, and refresh it once. Reopen Zinni.

IF IT STILL SHOWS THE OLD VERSION (Chrome / Edge)
1. Open the Zinni website in the browser.
2. Open Developer Tools (right-click the page > Inspect).
3. Go to Application > Service Workers, click Unregister for the Zinni service worker.
4. Go to Application > Storage and choose Clear site data (this can remove local browser-stored Zinni data, so export a backup first if you have tasks you need to keep).
5. Reload the site. The new service worker should register again.

DATA WARNING
Zinni task data is stored in local browser storage, not in the service worker cache. A normal hard refresh should preserve it. Clearing all site data may delete it; export a backup from Settings first.

NEW INSTALLS
The app remains a static GitHub Pages site and can be installed through a supported browser when served over HTTPS. The service worker supports offline use of cached assets, while online page navigation checks for newer HTML first.
