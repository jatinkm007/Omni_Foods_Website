# Omni_Foods_Website

# OmniFoods

OmniFoods is a responsive front-end marketing website for a healthy food delivery service. Built with plain HTML5 and CSS3 — no frameworks, no JavaScript, no build tools — it is a complete, multi-section landing page designed to take a visitor from first impression all the way to choosing a meal plan and signing up.

## Project Overview

The page is structured as a single scrollable narrative, where each section answers the next logical question a potential customer might have.

It opens with a **full-screen hero** featuring a fixed parallax background, a navigation bar, and two call-to-action buttons. The **features section** introduces four key selling points — 365-day availability, 20-minute delivery, 100% organic ingredients, and open ordering — each accompanied by an Ionicon icon. A **meal photo gallery** displayed across two rows of four images gives the service a visual, appetising identity, complete with zoom and opacity hover effects.

The **"How It Works"** section walks through the three-step ordering process alongside a phone app mockup and App Store / Google Play badges. A **Cities section** shows which locations OmniFoods currently serves, followed by a **Testimonials section** where three customer quotes appear over a dark fixed-background image. The **Pricing section** lays out three plans side by side — Premium ($399/month), Pro ($199/month), and Starter ($19/meal) — so a visitor can compare and decide at a glance. A **contact form** and a **footer** with social media links close out the page.

The visual design is built around the Lato typeface (loaded from Google Fonts), an orange accent colour (`#e67e22`), and a clean white background. Icons are provided by Ionicons v7.1.0 via CDN. CSS is split across four files with a clear separation of concerns: `normalize.css` handles cross-browser consistency, `grid.css` provides a custom float-based column system (supporting 2 through 12 column layouts), `queries.css` manages all responsive breakpoints, and `style.css` contains every design decision specific to OmniFoods.

## How to Run

There is nothing to install, compile, or configure. Because the project is pure HTML and CSS, you can open it directly in any web browser.

```bash
# On macOS
open index.html

# On Windows
start index.html

# On Linux
xdg-open index.html
```

Alternatively, you can drag the `index.html` file directly into a browser window. All local styles will load immediately. The only things that require an internet connection are the Google Fonts stylesheet and the Ionicons web component — so the typography and icons will only render correctly when you are online.

## Responsive Breakpoints

The site adapts to four screen size ranges, all defined in `queries.css`. Rather than targeting specific devices, each breakpoint targets a content width where the layout would otherwise start to break.

**1200px and below** is the widest breakpoint and makes the subtlest change: it reduces the horizontal padding on the main row containers and the hero text box, so content doesn't press uncomfortably against the edges on mid-sized laptops or large tablets in landscape mode.

**1023px and below** handles large tablets. At this size, the app phone mockup scales to 50% width, the pricing plan boxes expand to full width (three columns becomes too narrow to read comfortably), font sizes reduce to 18px, section padding tightens, and the contact form narrows to 80% of its container width.

**767px and below** is the most significant breakpoint, covering small tablets and large phones. The main navigation bar is hidden entirely at this width — adding a hamburger menu toggle here would be the natural next step if the project were taken further. All columns revert to full width and stack vertically, the body font size drops to 16px, and spacing values reduce throughout to keep things compact without feeling cluttered.

**480px and below** handles small phones. Section padding reduces to its minimum, the contact form expands to 90% of the screen width, and every grid column class produces 100% width — ensuring all content stacks cleanly in a single column on even the smallest screens.
