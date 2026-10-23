ZINNI — GITHUB PAGES DEPLOYMENT

FILES
Upload the files in this folder to the ROOT of your GitHub repository:
- index.html (the homepage)
- manifest.webmanifest (PWA install metadata)
- icon.svg (app icon)
- sw.js (offline service worker)
- .nojekyll (tells GitHub Pages not to run Jekyll)

PUBLISH
1. Sign in at https://github.com
2. Click + (top right) > New repository.
3. Name it zinni (or another name you like). For a GitHub Free account, choose Public.
4. Create the repository.
5. Click Add file > Upload files.
6. Unzip this package on your computer, then upload the FILES listed above from inside the folder. Do not upload the ZIP itself. Ensure index.html is at the repository root, not inside another folder.
7. Click Commit changes.
8. Open the repository's Settings > Pages.
9. Under Build and deployment, choose Deploy from a branch.
10. Choose branch main and folder /(root), then Save.
11. Wait for deployment. Return to Settings > Pages and click Visit site.

The address is usually https://YOUR-USERNAME.github.io/zinni/ (replace YOUR-USERNAME with your GitHub username; if you chose another repository name, use that name instead).

INSTALL
Open the published HTTPS website in Chrome or Edge, open Zinni's menu, and use Install Zinni as an app if available. You can also use the browser's install icon/menu. On iPhone/iPad Safari, use Share > Add to Home Screen.

NOTES
- GitHub Pages sites are public. Do not store secrets in this repository.
- The app saves planner data in local storage on that device/browser. It does not sync between devices. Export a backup from the app before clearing browser data.
- If you update the files later, upload the updated files and commit the changes. GitHub Pages may take a few minutes to publish.
