# PK Air Solutions — GitHub Pages Website

This is a responsive, single-file website for PK Air Solutions. It is designed to start on a free GitHub Pages address and can later use a purchased custom domain.

## Files
- `index.html` — the full website (HTML, CSS, and JavaScript in one file)

## Publish free with GitHub Pages
1. Sign in to https://github.com/
2. Create a **public** repository named `pk-air-solutions` (or another name you prefer).
3. Upload `index.html` to the repository root (the top-level folder).
4. Open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Choose branch `main` and folder `/(root)`, then click **Save**.
7. Wait for the deployment to finish. Your project site address will normally look like:
   `https://YOUR-GITHUB-USERNAME.github.io/pk-air-solutions/`
   Replace `YOUR-GITHUB-USERNAME` with your exact GitHub username. If you instead create a repository named `YOUR-GITHUB-USERNAME.github.io`, the address will be `https://YOUR-GITHUB-USERNAME.github.io/`.

Official guide: https://docs.github.com/en/pages/quickstart

## Important: update your contact details
In `index.html`, find the `CONTACT DETAILS` section near the bottom:
```js
const BUSINESS = {
  phoneDisplay: "8489530498",
  phoneDial: "+918489530498",
  whatsapp: "918489530498"
};
```
Edit these values if your contact number changes. WhatsApp must use digits only, including the country code (`91` for India).

## Replace sample gallery photos
The gallery currently uses sample countryside photos from Unsplash. Replace those with your own photos when possible:
1. Create an `images` folder in the repository.
2. Upload images you own or have permission to use, for example `drone-spraying.jpg`.
3. In `index.html`, replace the relevant sample image URL with `images/drone-spraying.jpg`.
4. Commit the changes. GitHub Pages will publish the update.

## Add more services later
Find the `<!-- FUTURE SERVICE CARD ... -->` comment in `index.html`. Copy an existing `<article class="service-card">...</article>` block and edit its title, description, and `data-service` value. If you add a new form service, also add a matching `<option>` inside the form's `<select id="service">`.

## How the enquiry form works
The form prepares a WhatsApp message and opens it for the visitor to review and send. It does not store submissions and does not require a backend. A visitor must have WhatsApp available to send the message.

## Custom domain later
When you buy a domain, configure it in **Repository → Settings → Pages → Custom domain**, then follow GitHub's DNS instructions from your domain provider:
https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site

Do not add DNS records until you have added the custom domain in the GitHub Pages settings. DNS changes may take time to propagate.

## Privacy and safety
GitHub Pages sites are public. Do not commit passwords, private customer information, or secret keys to the repository. Review all public contact details and photos before publishing.
