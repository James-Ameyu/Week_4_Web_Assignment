# SpendWise Dashboard Shell

SpendWise is a personal finance dashboard designed to provide a clear overview of income, expenses, savings, and spending categories.

This version is the Week 4 visual foundation of the project. It uses static content only and does not yet include JavaScript functionality.

## Files

- `index.html` - Contains the structure and content of the dashboard.
- `style.css` - Contains the dashboard styling, layout, responsive design, theme variables, and card interactions.

## Features

### Dashboard Layout

The dashboard contains:

- A SpendWise sidebar/navigation menu
- A main dashboard header
- Available balance information
- A summary of income, expenses, and savings
- Six spending category cards:
  - Food
  - Transport
  - Rent
  - Entertainment
  - Savings
  - Utilities

### CSS Grid

CSS Grid is used for the overall dashboard layout.

The desktop layout contains:

- A fixed-width sidebar
- A flexible main content area

CSS Grid is also used for the six category cards.

### Flexbox

Flexbox is used inside several parts of the dashboard, including:

- Sidebar navigation
- Header content
- Profile information
- Summary cards
- Category cards
- Card content and progress indicators

No absolute positioning is used for the page layout.

### CSS Custom Properties

The `:root` selector contains the main application theme variables, including:

- Brand color
- Accent color
- Surface color
- Background color
- Primary text color
- Secondary text color
- Border color
- Success and danger colors

Using CSS variables makes the theme easier to maintain and update.

### Responsive Design

A media query at `max-width: 767px` changes the desktop dashboard into a single-column mobile layout.

On smaller screens:

- The sidebar moves above the main content.
- Navigation items become a flexible row.
- Summary cards stack vertically.
- Category cards become a single-column grid.
- Header content stacks vertically.

The layout can be tested using the browser's DevTools Device Toolbar.

### Card Micro-interactions

The category cards include both mouse and keyboard interactions.

On hover or keyboard focus, cards:

- Move upward slightly using `transform`
- Gain a subtle `box-shadow`
- Change their border color

The transition duration is 200ms, which is below the required 250ms maximum.

The cards use `tabindex="0"` so they can also receive keyboard focus.

### Dark Theme

As a stretch goal, a dark theme is included using:

```css
@media (prefers-color-scheme: dark)


Only the CSS custom property values are overridden to create the dark color scheme.

How to Run

Clone or download this repository.

Open index.html in a browser.

Use the browser's DevTools to inspect the layout.

Open the Device Toolbar to test the responsive layout at different screen sizes.

Technologies

HTML5

CSS3

CSS Grid

Flexbox

CSS Custom Properties

CSS Media Queries

:::

### Quick submission checklist

- [x] `index.html`
- [x] `style.css`
- [x] `README.md`
- [x] Sidebar/navigation
- [x] Header
- [x] Six financial category cards
- [x] CSS Grid for the dashboard
- [x] Flexbox inside dashboard components
- [x] No absolute positioning
- [x] CSS custom properties on `:root`
- [x] Responsive single-column layout below 768px
- [x] Card hover interaction
- [x] Card keyboard focus interaction
- [x] 200ms transitions
- [x] Dark-theme stretch goal
- [x] Realistic static financial content

Before submitting, open the page in your browser and use **DevTools → Device Toolbar** to verify the desktop and mobile layouts yourself.
