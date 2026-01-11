Personal Portfolio - K.N.V.S.R Abijith

Project Overview

This project is a fully responsive personal portfolio website designed for K.N.V.S.R Abijith, an AI & ML Engineer. The site serves as a professional digital resume to showcase technical skills, academic achievements, certifications, and key projects like the "Sanjaya" robotic agent and Reddit toxicity detection system.

Objectives:

Professional Presence: Create a polished online identity using a modern "Shiny Blue" aesthetic.

Responsiveness: Ensure seamless accessibility across Mobile, Tablet, and Desktop devices.

Showcase: Effectively present projects with direct links to GitHub repositories and a comprehensive list of certifications.

Design Aesthetic

Theme: "Shiny Blue" / Cyber Tech.

Palette: Electric Blue (#2563EB) to Cyan gradients on a light background with deep navy contrasts.

Effects:

Glassmorphism: Frosted glass headers for a modern feel.

Glow: Soft blue shadows on buttons, cards, and profile images.

Gradients: Metallic text fills and button backgrounds.

Setup Instructions

Prerequisites

A code editor (VS Code recommended).

A modern web browser (Chrome, Firefox, Edge).

Git installed on your machine.

Installation & Configuration

Clone the Repository:

git clone [https://github.com/Abijith44/week1-portfolio.git](https://github.com/Abijith44/week1-portfolio.git)


Navigate to Folder:

cd week1-portfolio


Image Placement:

Ensure your profile picture is named profile.png (or profile.jpg) and placed in week1-portfolio/images/.

Ensure the favicon is named icon.jpg and placed in week1-portfolio/images/.

Resume Placement:

Place your PDF resume named Abijith_Resume.pdf in the root week1-portfolio/ folder.

Run: Open index.html directly in your browser or use the "Live Server" extension in VS Code.

Code Structure

The project follows a standard front-end development structure:

week1-portfolio/
│── index.html          # Main entry point; contains semantic HTML5 markup
│── css/
│   ├── variables.css   # CSS Variables for the "Shiny Blue" palette
│   ├── style.css       # Core styling, gradients, glassmorphism, and layouts
│   └── responsive.css  # Media queries for tablet and mobile adaptations
│── js/
│   └── navigation.js   # JavaScript for mobile menu and mailto form handler
│── images/
│   ├── profile.png     # User Profile Image
│   ├── icon.jpg        # Website Favicon
│   └── icons/          # (Optional) Additional assets
├── Abijith_Resume.pdf  # PDF Resume
├── .gitignore          # Git configuration
└── README.md           # Project documentation


Visual Documentation

Features Demonstrated

Hero Section: Features a glowing profile image, gradient text, social links, and call-to-action buttons.

Navigation: A sticky, glassmorphism header that transforms into a hamburger menu on mobile devices.

Grid Layouts: Used in "Skills", "Projects", and "Certifications" sections to create responsive cards.

Interactive Cards: Project cards hover with a glow effect and link directly to GitHub.

Contact Form: A functional form layout that uses JavaScript to open the user's default email client with pre-filled details.

Technical Details

Architecture

The website utilizes a component-based architecture within a single page (SPA feel):

HTML5: Uses semantic tags (<header>, <nav>, <section>, <article>) to improve SEO and accessibility.

CSS3:

Variables: Colors (--primary-color, --accent-glow) are defined in variables.css for consistent theming.

Flexbox & Grid: Used extensively for layout management.

Backdrop Filter: Used for the glassmorphism effect in the header.

JavaScript: Pure DOM manipulation is used for the mobile menu toggle and the mailto form handling.

Algorithms (Navigation Logic)

Toggle Mechanism: Event listener detects clicks on the hamburger icon -> Toggles CSS class active on the nav menu.

Scroll Spy: window.onscroll calculates the current scroll position against section offsets to highlight the active link.

Mail Handler: Intercepts form submission -> Constructs a mailto: URL with user input -> Redirects window location to open email client.

Testing Evidence

Validation

HTML: Validated using W3C standards; all tags are properly closed and nested.

CSS: Vendor prefixes used where necessary; layout tested on Chrome and Edge.

Contact Form: Inputs have required attributes to prevent empty submissions.

Test Cases

Mobile View (375px):

Test: Click Hamburger icon.

Result: Menu slides in; links are clickable.

Tablet View (768px):

Test: Check Project Grid.

Result: Grid adjusts from 3 columns to 2 columns or 1 column stack.

Desktop View (1200px):

Test: Click Project Card.

Result: Opens specific GitHub repository in a new tab.

Functionality:

Test: Click "Send Message".

Result: Opens default mail app with "Portfolio Contact" subject line.
