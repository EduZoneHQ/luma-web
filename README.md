# Nexora Digital website

A responsive, static landing page for the proposed Nexora Digital brand. The site is currently a single `index.html` file with inline CSS and JavaScript. There is no build step or package manager.

## What is included

- Public service information for web development, graphic design, video editing, CVs and documents, presentations, tutoring, social media management, and tech support.
- Suggested naira starting rates. Confirm scope, availability, delivery time, and final pricing before accepting work.
- Website package pricing, sample portfolio concepts labelled as demos, contact forms, and responsive layouts.
- Existing Supabase-backed client login, portal, lead collection, and private admin area.

The Nexora Digital name is provisional and should be confirmed before merging or publishing this branch. Sample portfolio items are concepts, not client work.

## Preview on a ThinkPad T490 with VS Code

1. Install Git and Visual Studio Code if they are not already installed.
2. In VS Code, choose **Source Control → Clone Repository**.
3. Enter `https://github.com/EduZoneHQ/luma-web.git`, select the `codex/nexora-digital-site` branch when prompted, and open the cloned folder.
4. Open `index.html`. For a local preview, install the free **Live Server** extension, right-click `index.html`, and choose **Open with Live Server**. You can also open the file directly in a browser.
5. Edit and save `index.html`; the browser preview refreshes automatically with Live Server.

## Free deployment

After confirming the brand and merging the branch into `main`, GitHub Pages can host this static site at no charge:

1. In the repository, open **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and the `/(root)` folder, then save.
3. Wait for the Pages URL shown on that settings page.
4. In the Supabase project’s Auth URL settings, add the published site URL to the allowed redirect URLs if client login is being used. Keep the local preview URL allowed during development as needed.

This repository has no `package.json`, build command, or hosting configuration. GitHub Pages serves `index.html` directly.

## Supabase and secrets

The existing browser-side Supabase integration and data model are preserved. Do not place a Supabase service-role key, database password, or other private credential in this public repository or in browser code. Keep database access protected by appropriate Supabase policies. Contact details and the WhatsApp destination should be verified by the owner before the site is published.
