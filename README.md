# Fruitkha

A responsive single-page fruit shop experience built with HTML, Tailwind CSS utilities, and vanilla JavaScript.

## Features

- Fully responsive fruit shop landing page with a coastal navy, teal, and yellow visual palette
- Fluid hero typography, mobile-safe buttons, responsive product and benefits grids, and flexible footer controls
- Desktop navigation and fixed mobile drawer navigation
- Section links for Home, About, Shop, News, Contact, and Cart
- Product cart counter with add-to-cart notifications
- Newsletter email validation and confirmation message
- Local image assets with external Font Awesome icons

All page styling, responsive breakpoints, drawer states, hover effects, and layout utilities are implemented with Tailwind CSS. No custom CSS stylesheet is required.

## Page Sections

The navigation uses in-page anchors so visitors can move through the single page without broken placeholder links:

| Link | Section |
| --- | --- |
| Home | Hero section |
| About | Brand story and testimonial |
| Shop | Product collection |
| News | Seasonal sale banner |
| Contact | Footer contact and newsletter area |
| Cart | Cart interaction anchor |

## Run Locally

No build step is required because the page loads Tailwind CSS from its CDN.

From the project directory, run:

```powershell
python -m http.server 8000
```

Then open [http://localhost:8000/Fruitkha.html](http://localhost:8000/Fruitkha.html).

The layout is designed for mobile, tablet, and desktop screens. Product cards use one column on small screens, two columns on medium screens, and three columns on large screens.

## Deploy

The repository includes `index.html`, which redirects to `Fruitkha.html` so GitHub Pages can use the repository root as its entry point.

### GitHub Pages

1. Create a GitHub repository and push these files to the `main` branch.
2. Open the repository's **Settings > Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the `main` branch and the `/ (root)` folder, then click **Save**.
5. Open the published Pages URL after GitHub finishes the deployment.

The page loads Tailwind CSS and Font Awesome from CDNs, so visitors need internet access for styling and icons. Page images are stored locally in `assets/images` and do not depend on the original external image host.

## Files

```text
index.html     # GitHub Pages root entry point
Fruitkha.html  # Main page, Tailwind utilities, and JavaScript interactions
assets/images/ # Local hero, product, profile, sale, and logo images
README.md      # Project documentation
```