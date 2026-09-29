# DevPulse Cloud Infrastructure

## Assignment 1B — DevPulse Cloud Telemetry Landing & Responsive Pricing Dashboard

DevPulse is a responsive cloud infrastructure SaaS landing page designed to showcase cloud telemetry, infrastructure monitoring, log aggregation, and automated remediation services.

This project translates the semantic structure and usability planning from Assignment 1A into a production-style HTML5 and CSS3 responsive landing page.

## Features

* Responsive cloud infrastructure landing page
* Semantic HTML5 document structure
* Infrastructure monitoring feature cards
* Responsive cluster hosting pricing tiers
* Featured "Pro Cluster" pricing tier
* Workload infrastructure estimator
* API Sandbox registration form
* Native HTML5 form validation
* Interactive hover and keyboard focus states
* Responsive layout for desktop and mobile screens
* No JavaScript or CSS frameworks

## Technologies Used

* HTML5
* CSS3
* Flexbox
* CSS Grid
* CSS Media Queries
* CSS Custom Properties
* HTML5 Form Validation
* Git and GitHub

## Project Structure

```text
devpulse-dashboard/
│
├── index.html
├── style.css
└── README.md
```

## Page Sections

### Hero Section

The hero section introduces the DevPulse cloud infrastructure platform and provides primary calls to action for deploying a free cluster or viewing pricing.

### Infrastructure Features

The features section highlights three primary DevPulse capabilities:

* Latency Tracking
* Log Aggregation
* Auto-Remediation

Each feature provides a list of platform capabilities.

### Workload Estimator

The workload estimator allows users to enter infrastructure requirements such as:

* Node count
* Log throughput
* Storage requirements
* Deployment environment
* Monitoring level
* Backup requirements

The form uses native HTML5 validation and input constraints.

### Cluster Hosting Tiers

The pricing section provides three hosting tiers:

* Developer
* Pro Cluster
* Enterprise Dedicated

The Pro Cluster tier is visually highlighted as the recommended option.

### API Sandbox Registration

The registration section allows users to provide account information and select configuration preferences, including:

* Full name
* Email address
* Company or organization
* Account type
* Preferred deployment region
* Product update preferences
* Beta feature notifications
* Terms and conditions agreement

## Responsive Design

The page is designed to adapt to different screen sizes using CSS media queries.

Flexbox is used for one-dimensional layouts such as the navigation, hero content, buttons, and footer.

CSS Grid is used where appropriate for two-dimensional content layouts such as feature and pricing sections.

The mobile layout is designed to collapse content into a single-column layout at smaller viewport widths.

## Accessibility and Native Validation

Form controls use associated `<label>` elements with matching `for` and `id` attributes.

Native HTML5 validation is used instead of JavaScript. Numeric inputs use constraints such as:

```html
required
min="1"
max="1000"
step="1"
```

Email inputs use:

```html
type="email"
required
```

Interactive buttons and links also provide visual feedback through CSS `:hover` and `:focus-visible` states.

## Design System

The project uses CSS custom properties to maintain a consistent visual theme.

The design system includes variables for:

* Background colors
* Card colors
* Primary buttons
* Hover states
* Main and secondary text
* Borders
* Accent colors
* Font family
* Transition timing

This allows the visual appearance of the site to be modified without changing individual components.

## Git Version Control

The project is developed using Git with progressive commits rather than a single monolithic commit.

Example commit structure:

```text
feat: add semantic landing page structure
style: add navigation and hero layout
feat: add pricing and workload sections
style: update color palette and visual theme
style: add responsive layout and interaction states
```

Each commit represents a meaningful stage of development.

## Assignment Requirements

This project was created for Assignment 1B and follows the required HTML5 and CSS3 implementation approach.

The project does not use:

* JavaScript
* Bootstrap
* Tailwind CSS
* Other CSS frameworks

The final repository contains the required project files and is intended to be submitted as a public GitHub repository.


## Rubric

| Category                                 | Requirements                                                                                    | Implementation                                                                                                                                                                                                         |
| ---------------------------------------- | ----------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Semantic HTML5 & Structure**           | Use semantic landmarks and maintain proper heading hierarchy.                                   | **Completed:** The page uses `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, and `<footer>`. The heading hierarchy follows an `h1 → h2 → h3` structure.                                                       |
| **CSS Layout: Flexbox & Grid**           | Use Flexbox and CSS Grid to create responsive layouts.                                          | **Completed:** Flexbox is used for navigation, hero content, buttons, forms, and footer layouts. CSS Grid is used for the feature and pricing card layouts, with responsive columns that collapse on smaller screens.  |
| **Featured Tier & Interactive Feedback** | Clearly identify the featured pricing tier and provide interactive feedback through CSS states. | **Completed:** The Pro Cluster tier is identified with a "Most Popular" marker and distinct styling. Buttons and navigation elements use `:hover` and `:focus-visible` states to provide visual feedback.              |
| **Native Form Validation**               | Use HTML5 form controls and native validation without JavaScript.                               | **Completed:** Forms use native HTML validation including `required`, `type="email"`, `type="number"`, `min`, `max`, and `step` attributes. No JavaScript is used for validation.                                      |
| **Responsive Design**                    | Support mobile layouts and prevent horizontal overflow.                                         | **Completed:** Media queries are used to adapt the layout for smaller screens. Feature and pricing grids collapse to a single-column layout on mobile devices.                                                         |
| **Design System & CSS Organization**     | Use CSS custom properties and consistent styling.                                               | **Completed:** CSS custom properties are used for colors, typography, borders, and transition timing. Shared button, card, form, and layout styles reduce repetition and maintain consistency.                         |
| **Accessibility**                        | Provide accessible form labels and usable interactive elements.                                 | **Completed:** Form controls have associated `<label>` elements using matching `for` and `id` attributes. Interactive elements provide visible hover and keyboard focus feedback.                                      |
| **Git Version Control**                  | Maintain at least four meaningful commits across distinct development sessions.                 | **Completed:** The project is developed using Git with descriptive commits documenting major stages of development, including semantic HTML, layout/styling, pricing and workload sections, and visual design updates. |
| **Documentation**                        | Include a clear README and maintain a clean project structure.                                  | **Completed:** This README documents the project purpose, technologies, features, responsive design, accessibility, design system, and development process.                                                            |
| **No Frameworks or JavaScript**          | Build the project using HTML5 and CSS3 without CSS frameworks or JavaScript.                    | **Completed:** The project uses only HTML5 and CSS3. No CSS framework or JavaScript is required.                                                                                                                       |
