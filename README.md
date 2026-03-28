# Upendo Inn

A hotel check-in and suite booking landing page for **Upendo Inn** accommodation facility. Guests can fill in their details and select a preferred suite type to begin the booking process.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Known Limitations](#known-limitations)

---

## Overview

Upendo Inn is a front-end landing page that presents guests with a welcoming sign-in form. The page features a full-screen lodge background image and a centrally positioned booking form where guests can enter their personal details and choose from four suite categories.

---

## Features

- Welcoming hero layout with a full-screen lodge background image
- Guest information form with the following fields:
  - Full Name
  - Username
  - Email address
  - Phone number
  - Suite type selection (Standard, Deluxe, Premium, Executive)
- Confirmation prompt before form submission
- Responsive viewport meta tag for mobile compatibility

---

## Tech Stack

| Technology | Purpose               |
|------------|-----------------------|
| HTML5      | Page structure & form |
| CSS3       | Styling & layout      |
| JavaScript | Confirmation dialog   |

No external libraries, frameworks, or build tools are required.

---

## Project Structure

```
upendoinn/
├── index.html       # Main landing page and booking form
├── index.css        # Stylesheet for layout and visual design
├── LodgePic2.jpg    # Background image used by the page
└── README.md        # Project documentation
```

---

## Getting Started

### Prerequisites

All you need is a modern web browser. No installation or build step is required.

### Running Locally

**Option 1 – Open directly in a browser:**

```bash
# Clone the repository
git clone https://github.com/Moses1320/upendoinn.git
cd upendoinn

# Open the page (macOS)
open index.html

# Open the page (Linux)
xdg-open index.html

# Open the page (Windows)
start index.html
```

**Option 2 – Serve with a local HTTP server (recommended for form testing):**

```bash
# Python 3
python -m http.server 8000

# Node.js (if http-server is installed)
npx http-server
```

Then navigate to `http://localhost:8000` in your browser.

---

## Usage

1. Open `index.html` in a browser.
2. Fill in your **Full Name**, **Username**, **Email**, and **Phone** number.
3. Select your preferred **Suite Type** from the dropdown:
   - Standard
   - Deluxe
   - Premium
   - Executive
4. Click **Send**. A confirmation dialog will appear.
5. Confirm to submit the form.

---

## Known Limitations

- The form's `action` attribute points to `index.php`, which does not yet exist in the repository. Form submissions will fail until a backend handler is added.
- There is no input validation beyond the browser's built-in `required` attribute checks.
- No database or server-side logic is currently implemented.
