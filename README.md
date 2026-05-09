# Dawn Practice — Custom Shopify Theme Development

A custom Shopify theme built on top of Shopify's Dawn framework, developed as part of my Shopify development learning journey. This project demonstrates core Shopify theme development skills including Liquid templating, schema settings, responsive CSS, JavaScript, and the Shopify Ajax API.

## Live Preview
Built and tested on a Shopify Partner development store using the Shopify CLI local development server.

## Custom Sections Built from Scratch

### 1. Announcement Bar
- Dismissible top banner with cookie persistence
- Closes on click and stays hidden for 7 days via browser cookie
- Editable message, background color, and text color via schema settings

### 2. Promo Banner
- Full-width promotional banner with editable heading, subtext, and background color
- Merchant-customizable via Shopify theme editor

### 3. Featured Product
- Displays a single product with image, title, price, and Add to Cart button
- Integrated with cart drawer via Shopify Ajax API
- "View Full Details" link to full product page
- Fully responsive — stacks vertically on mobile

### 4. Product Grid
- Displays products from a selected collection in a 3-column responsive grid
- Merchant can select collection and number of products via schema settings
- Responsive: 2 columns on mobile

### 5. Newsletter Signup
- Email capture form using Shopify's built-in customer form
- Displays success message on submission and error handling
- Fully editable title, subtext, placeholder, and button text

### 6. Ajax Cart Drawer
- Slide-out cart panel using Shopify's Cart Ajax API (`/cart.js`, `/cart/add.js`, `/cart/change.js`)
- Opens automatically when a product is added to cart
- Displays product image, title, quantity, and line price
- Remove items without page reload
- Shows cart total and Checkout button
- Closes on overlay click or ✕ button

## Tech Stack
- Shopify Liquid
- HTML5 / CSS3
- Vanilla JavaScript
- Shopify Ajax Cart API
- Shopify CLI
- Git / GitHub

## Skills Demonstrated
- Shopify theme architecture (layouts, sections, snippets, templates)
- Liquid templating — objects, tags, filters
- Section schema settings (text, color, product, collection, range)
- Responsive design with CSS Grid and Flexbox
- JavaScript DOM manipulation and event handling
- Shopify Ajax API integration
- Cookie-based UI state persistence
- Git version control workflow

## Setup
1. Install Shopify CLI: `npm install -g @shopify/cli @shopify/theme`
2. Clone this repo: `git clone https://github.com/Binzzzzzzzzzzzz/dawn-practice.git`
3. Run dev server: `shopify theme dev --store YOUR-STORE.myshopify.com`