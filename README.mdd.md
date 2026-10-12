# Hunar – Freelancing Marketplace Platform

Hunar ("skill" in Urdu) is a freelancing marketplace where clients can find freelancers for web, design, mobile, data and marketing work. Built as an internship project with HTML5, CSS3 and vanilla JavaScript.

- **Week 1:** landing page (homepage)
- **Week 2:** freelancer and service marketplace interface (browse, search, filter, sort, profile page)

## Features

### Week 1 – Landing page

- **Navigation bar:** brand logo, Home, Find Freelancers, Find Jobs, About, and Login/Register buttons. It stays fixed at the top, highlights the section you are viewing, and becomes a hamburger menu on mobile.
- **Hero section:** platform introduction, a tabbed search bar ("Search for services" / "Search freelancers"), quick-search tags, and animated platform stats.
- **Popular categories:** Web Development, Graphic Design, Mobile App Development, Data Analysis and Digital Marketing.
- **How it works:** three-step explanation of the platform.
- **Featured freelancers:** cards generated from a JavaScript data array, with live search, category chips, sorting and a save (heart) button.
- **Login/Register modal:** form validation, switch between login and register, closes with Esc or a click outside.
- **Footer:** links and copyright.

### Week 2 – Marketplace interface

**Find Freelancers page (`freelancers.html`)**

- **Freelancer/service cards:** each card shows a profile image, freelancer name, city, service title, category, starting price, rating, number of reviews, and a **View Profile** button. Cards are built by one reusable function.
- **Search:** live search by name, service, skill or category (for example "react" or "logo design").
- **Category filtering:** filter chips for all five categories.
- **Advanced filters:** maximum starting price slider and minimum rating.
- **Sorting:** Highest Rated, Price: Low to High, Price: High to Low, and Most Reviews.
- **Dynamic content handling:** result count that updates instantly, a loading skeleton, an empty state with a "Clear filters" button, and saved freelancers that are remembered in the browser.

**Freelancer Profile / Service Details page (`profile.html`)**

- Opens from the **View Profile** button using the freelancer's id in the link (for example `profile.html?id=3`).
- Profile header with image, name, service title, rating, city and category.
- **About** and **Reviews** tabs, with skills and sample reviews.
- **Basic, Standard and Premium packages:** the price, delivery time and included features change when a package is selected.
- **Multiple UI states:** loading skeleton, profile view, "not found" message, request sending, and request sent confirmation.
- **Save** button and a "You may also like" section with more freelancer cards.

**Both weeks**

- **Responsive design:** desktop, tablet (up to 960px) and mobile (up to 700px). The freelancer grid changes from 4 columns to 3, 2 and 1.
- **Consistent design:** the same colours, fonts, buttons and navigation as the Week 1 landing page.
- **Accessibility:** keyboard focus styles, ARIA labels, and reduced-motion support.

## Technologies

- HTML5
- CSS3 (Grid, Flexbox, CSS variables, media queries)
- JavaScript (DOM manipulation, event delegation, URL parameters, localStorage, IntersectionObserver)

## Project structure

```
├── index.html         # Week 1: landing page
├── style.css          # Week 1: main design and responsive styles
├── main.js            # Week 1: landing page interactions
├── freelancers.html   # Week 2: Find Freelancers page
├── profile.html       # Week 2: freelancer profile / service details page
├── market.css         # Week 2: styles for the marketplace and profile pages
├── common.js          # Week 2: sample freelancer data, reusable card, navigation
├── market.js          # Week 2: search, filtering and sorting
└── profile.js         # Week 2: profile page, tabs, packages and order states
```

## How to run

1. Download or clone the repository.
2. Keep all files in the same folder.
3. Open `index.html` in a browser (or use the VS Code Live Server extension), then click **Find Freelancers**.

## Screenshots

Add your desktop, tablet and mobile screenshots here, for example:

```
![Home page](screenshots/home.png)
![Find Freelancers](screenshots/freelancers.png)
![Freelancer profile](screenshots/profile.png)
![Mobile view](screenshots/mobile.png)
```

## Author

Fazeela Manzoor ([@Fazeela594](https://github.com/Fazeela594))
