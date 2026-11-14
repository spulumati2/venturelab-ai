# VentureLab — Free Venture Capital Simulator

VentureLab is a browser-based educational game for learning how venture capital investors evaluate fictional startups, calculate ownership, and manage a simulated fund. It uses plain HTML, CSS, and JavaScript: no build step, paid API, subscription, or server is required.

## Included features

- Responsive desktop and mobile layout.
- $10,000,000 virtual starting fund.
- Startup marketplace with search and industry filters.
- Randomized fictional startup generator.
- Deal review with founder, business model, revenue, growth, margin, valuation, and risks.
- Investment calculator using pre-money and post-money valuation.
- Portfolio ownership and paper-value tracking.
- Quarterly simulation with randomized illustrative valuation changes.
- Simulated exits that return virtual proceeds to available fund capital.
- Export and import game progress as a JSON save file.
- Six VC Academy lessons and XP progression.
- Built-in mentor for valuation, ownership, dilution, diligence, burn/runway, MOIC/IRR, founders, and portfolio review.
- Browser local-storage saves and basic offline caching as a PWA.
- Privacy notice and MIT license.

## Important: what “AI” means in this free edition

This version does not connect to a generative AI model. The startup generator uses randomized templates, and the mentor uses a curated rule-based knowledge base. They work without API keys, paid credits, or external services, but they are not equivalent to a fully conversational AI model. All company names, founders, metrics, valuations, and outcomes are fictional.

## Run and test locally

1. Download and extract the ZIP.
2. Open `index.html` in a current browser. Core gameplay works directly from the file.
3. To test PWA/offline support, run a local static server from this folder, for example `python -m http.server 8000`, then visit `http://localhost:8000`.

No `npm install`, Node server, API key, or environment variables are required.

## Publish free with GitHub Pages

GitHub Pages is available for public repositories on GitHub Free. A public repository means the source code is visible to everyone. Do not include private information, passwords, API keys, or personal data. See GitHub's current [Pages documentation](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site).

1. Sign in to GitHub and create a **new public repository** named `venturelab-ai`.
2. Extract the ZIP on your computer.
3. Open the repository and choose **Add file → Upload files**.
4. Open the extracted `venturelab-ai-free` folder on your computer and upload its *contents* (including `index.html`, `styles.css`, `app.js`, `privacy.html`, `manifest.webmanifest`, `sw.js`, `assets/`, `.nojekyll`, `LICENSE`, and `README.md`) into the repository's top level. Do not upload only the ZIP file.
5. Commit the uploaded files to the `main` branch.
6. In the repository, open **Settings → Pages**.
7. Under **Build and deployment**, choose **Deploy from a branch**.
8. Choose branch `main`, folder `/(root)`, then click **Save**.
9. Wait for the Pages deployment to finish. Return to **Settings → Pages** and open the published site link. Initial publishing can take several minutes.
10. Test the live site on desktop and mobile. Test startup generation, investments, quarter advancement, exit, lessons, mentor, export/import, and the privacy link.

GitHub's official instructions: [Create a Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site) and [configure publishing from a branch](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

## How the game works

- Start with $10M in virtual capital.
- Review a startup and choose an investment amount and pre-money valuation.
- Ownership = investment amount ÷ (pre-money valuation + investment amount).
- Your virtual cash decreases by the investment amount.
- Advance a quarter to simulate uncertain changes in company paper values. The simulation uses randomized outcomes and is not a forecast.
- Simulate an exit to move the current paper value back into virtual fund cash.
- Export your save regularly if you want a backup or want to move progress to another browser/device.

## Data, privacy, and limitations

- Game state is saved in the browser's `localStorage`; it is not synced across devices.
- Clearing browser site data may erase game progress. Export a save file for backup.
- No accounts, cloud database, analytics, or external API requests are included.
- The app is a static web app/PWA, not a native iOS or Android app. Users can open it in a mobile browser and may be able to install it from the browser's install/share menu.
- All financial outcomes are simulated. This is educational software, not investment advice, a real fund, or a prediction of investment performance.

## Before sharing publicly

- Replace the generic project description/branding if you want a different identity.
- Check the privacy notice and README still accurately describe the app.
- Test the published site and keep a backup of your source files.
- GitHub Pages sites are public; never put secrets or personal information in the repository.
