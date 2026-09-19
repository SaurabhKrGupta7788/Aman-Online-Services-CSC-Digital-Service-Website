# Aman Online Services: CSC Digital Storefront

A responsive, static digital storefront for a Common Service Centre (CSC) offering government and digital services. Built purely with HTML, CSS, and Vanilla JavaScript to ensure maximum performance, accessibility, and zero-maintenance hosting.

## Architecture Overview

```text
Client Web Browser
    │
    ▼
┌──────────────────────────┐
│  Static Asset Delivery   │  ← Served via GitHub Pages / CDN
└──────────┬───────────────┘
           │
    ┌──────┼───────────────┐
    ▼      ▼               ▼
┌───────┐ ┌─────────────┐ ┌─────────────┐
│ HTML5 │ │ CSS3 Flex/  │ │ Vanilla JS  │
│ DOM   │ │ Grid Styles │ │ Interactions│
└───┬───┘ └──────┬──────┘ └──────┬──────┘
    │            │               │
    ▼            ▼               ▼
┌───────────────────────────────────────┐
│  Rendered User Interface (UI)         │
│  - Service Catalog                    │
│  - Document Requirements              │
│  - Contact / Location Info            │
└───────────────────────────────────────┘
```

## System Output

The website visually outputs a categorized list of services for end-users:

| Service Category | Examples | Target User |
|---|---|---|
| Government IDs | PAN Card, Aadhaar Updates, Voter ID | General Public |
| Financial Services | Money Transfer, Bill Payments, Insurance | Local Residents |
| Academic | Scholarship Forms, Exam Registrations | Students |

## Directory Structure

```text
Aman-Online-Services-CSC-Digital-Service-Website/
├── index.html            # Main landing page
├── services.html         # Detailed list of CSC services
├── contact.html          # Location and contact forms
├── assets/               # Static images and icons
├── css/
│   └── style.css         # Responsive styling
├── js/
│   └── main.js           # Navigation toggles and UI scripts
└── README.md             # Project documentation
```

## How to Run

### 1. Prerequisites
- A modern web browser.

### 2. Run the Application
This is a purely static website with no backend dependencies.
1. Simply double-click `index.html` to open it in your browser.
2. Alternatively, for a better development experience, use a local server:
   ```bash
   python -m http.server 8000
   ```
   Then navigate to `http://localhost:8000`.

### 3. Usage
- Users can navigate through the site to view the digital services provided by the CSC.
- The site is fully responsive and will adapt to mobile and desktop screens.

## Key Design Decisions

1. **Zero Backend Dependency**: By using purely static files, the website can be hosted entirely for free on platforms like GitHub Pages, Vercel, or Netlify with infinite scalability and zero downtime.
2. **Vanilla Stack**: Avoiding heavy frameworks (like React or Angular) ensures the site loads instantly, which is critical for users accessing the site on slow, rural 3G/4G networks.
3. **Mobile-First CSS**: The layout is designed using CSS Flexbox and Media Queries to ensure readability on mobile devices, which represent the vast majority of the target demographic's internet usage.
