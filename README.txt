Bedrock Manifest Forge

Run locally on Windows:
1. Double-click start-local-server.bat.
2. Open http://localhost:8000 in your browser.

Deploy for free with GitHub Pages:
1. Create a GitHub repository for this project and upload all project files,
   including the .github/workflows folder and the PNG icons.
2. In the repository, open Settings > Pages and set the build and deployment
   source to GitHub Actions.
3. Ensure the default branch is named main, or edit the workflow's branch
   filter in .github/workflows/pages.yml to match your default branch.
4. Push the files to that branch, or run the "Deploy to GitHub Pages" workflow
   from the Actions tab using Run workflow.
5. Wait for the workflow to finish, then open the Pages URL shown in the
   workflow's deploy job or under Settings > Pages. A project site URL usually
   ends in /repository-name/.

The workflow publishes this folder as-is; no build tools or paid hosting are
needed. GitHub Pages serves the site over HTTPS, enabling installation as a
PWA and offline use after the first visit. The app processes pack data locally
in your browser and does not send it to a backend.

When installed, the app requests fullscreen display where the browser supports
it, then falls back to a standalone app window. Some browsers and operating
systems do not allow fullscreen PWAs; the layout centers itself when there is
enough space and adapts to smaller screens. After publishing display-mode
changes, close and reopen the installed app; if it keeps the old mode, remove
and reinstall it from the browser.
