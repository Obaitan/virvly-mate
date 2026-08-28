# VirvlyMate 📷

> **The photographs you take already have buyers. Most of them never find them.**

**VirvlyMate** is a modern, privacy-first, web-based platform tailored for roaming and itinerant photographers working in public or event spaces (such as beaches, landmarks, resorts, weddings, and parks). It streamlines the connection between photographers and clients, enabling customers to securely and instantly find themselves in photos using face-matching technology, and purchase high-quality digital copies on the spot.

---

## 🚀 How It Works

### For Photographers (The 5-Step Flow)
1. **Photograph**: Capture moments of people as you normally do, with no disruptions to your standard equipment or flow.
2. **Connect**: Provide clients with a photographer-specific code or a QR link so they know how to access their pictures.
3. **Upload**: Upload your high-resolution photos directly to VirvlyMate from your phone or camera in seconds.
4. **Find & Buy**: Clients use their phone to search, discover, and purchase their photos.
5. **Get Paid**: Funds land directly into your connected payment account with zero invoicing, follow-ups, or manual tracking.

### For Customers (Find Your Photos)
1. **Access**: Visit the `/clients` route (the Photo Matcher page).
2. **Upload Selfie**: Upload a quick portrait or selfie.
3. **Input Code**: (Optional) Enter the photographer's code to narrow down the search.
4. **Discover**: The secure matching engine highlights only the photographs containing your face.
5. **Purchase**: Securely pay through the platform and download high-resolution copies instantly.

---

## 🛡️ Privacy Approach
Privacy is a core pillar of the VirvlyMate architecture:
- **No Selfie Storage**: Search selfies uploaded by customers are processed in-memory to generate temporary matching vectors and are **never stored** on our servers.
- **Targeted Matching**: Clients can only see and access photos that they are actually in, protecting the privacy of other individuals.

---

## 🛠️ Technology Stack

- **Framework**: [Astro (v4+)](https://astro.build/) — For content-focused, ultra-fast performance and component-based static or hybrid site generation.
- **Styles**: [Tailwind CSS](https://tailwindcss.com/) — Utility-first styling with a bespoke design system tokenized into `tailwind.config.mjs`.
- **Interactivity**: Clean Client-Side TypeScript and CSS-driven transitions (e.g. passive event scroll behaviors, drag-and-drop file upload zones).
- **Fonts**: Pre-connected Google Fonts loaded for optimal performance:
  - *Plus Jakarta Sans* (Headings & Brand)
  - *Inter* (Body text)

---

## 📂 Project Structure

```text
virvly-mate/
├── public/                 # Static assets served at the root URL path
│   ├── brand/              # SVG brand assets (favicon, official logo)
│   └── images/             # Marketing, hero, and illustration images
├── src/
│   ├── components/         # Reusable Astro components
│   │   ├── Button.astro    # Standardized system button
│   │   ├── Footer.astro    # Global site footer
│   │   ├── Header.astro    # Global header with scroll-based style transitions
│   │   ├── StepCard.astro  # Interactive step card for photographer workflows
│   │   └── WhereCard.astro # Location cards showcasing service targets
│   ├── layouts/
│   │   └── Layout.astro    # Main page layout containing global styles and <head> setup
│   └── pages/
│       ├── index.astro     # Photographer-focused home landing page
│       └── clients.astro   # Interactive Photo Matcher client application page
├── astro.config.mjs        # Astro configuration file
├── tailwind.config.mjs     # Custom Tailwind configuration (colors, spacing, transitions)
└── package.json            # Node project configuration and dependencies
```

---

## 🎨 Branding System
The branding system uses custom design tokens defined in the Tailwind configuration:
- **Brand Blue**: `#00759F` (Used for primary branding accent elements)
- **Brand Deep Blue**: `#053349` (Used for overlays and deep hero containers)
- **Brand Orange**: `#F78C1E` (Used for CTA highlights and active states)
- **Brand Charcoal**: `#1C1C1C` (Used for dark blocks/footers and headings)
- **Brand Ink**: `#232323` (Used for core body copy)
- **Brand Paper**: `#FFFFFF` (Main page background)

---

## 💻 Getting Started

### Prerequisites
Make sure you have [Node.js](https://nodejs.org/) installed (version 18.14.1 or higher is recommended).

### 1. Install Dependencies
Run the package installation command from the project root:
```bash
npm install
```

### 2. Run the Development Server
Launch the local development environment with hot reloading enabled:
```bash
npm run dev
```
The application will run locally, typically at [http://localhost:4321/](http://localhost:4321/).

### 3. Build for Production
Create an optimized production-ready bundle inside the `/dist` directory:
```bash
npm run build
```

### 4. Preview the Build
Locally preview the generated production build to verify functionality and performance:
```bash
npm run preview
```

---

## 📝 License
Concept copy for discussion and prototyping. All rights reserved.
