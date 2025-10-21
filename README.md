Frontend Portfolio WebsiteOverviewThis is a multi-page personal portfolio website built as part of a frontend development program. Starting from a single-card landing page (Stage 0), it has evolved into a responsive, accessible multi-page application (Stage 1). The site showcases semantic HTML, CSS for layouts and responsiveness, basic JavaScript for form validation, and adherence to accessibility best practices (WCAG guidelines).Key themes: Accessibility, Responsiveness, Semantic Structure, and User-Centric Design.Current Version: Stage 1 (October 21, 2025)
Technologies: HTML5, CSS3, Vanilla JavaScript
Deployment: Static site—serve via any web server (e.g., Live Server in VS Code, GitHub Pages).FeaturesHome Page (index.html)Single portfolio card (from Stage 0) with a welcoming message.
Basic navigation header linking to all pages.

Contact Us Page (contact.html)Interactive form with client-side validation:Required fields: Full Name, Email, Subject, Message (min 10 characters).
Email format validation (e.g., name@example.com).
Real-time error feedback and submission prevention for invalid inputs.
Success message on valid submission (form hides, confirmation shows).

Accessibility: Labeled inputs, ARIA attributes (aria-describedby, aria-live), keyboard navigation, focus indicators.
Data-testids for testing: test-contact-name, test-contact-email, etc.

About Me Page (about.html)Reflective content sections: Bio, Goals, Areas of Low Confidence, Note to Future Self, Extra Thoughts.
Semantic structure using <main>, <section>, <h2>, <ul>, <p>.
Data-testids for testing: test-about-bio, test-about-goals, etc.

GeneralNavigation: Consistent header with links to Home, Contact Us, About Me.
Responsiveness: Mobile-first design with media queries:Mobile (≤768px): Stacked layouts, larger touch targets.
Tablet (769px–1024px): Horizontal form groups, adjusted spacing.
Desktop (≥1025px): Grid layouts for sections, wider content.

Accessibility: Semantic HTML, labels linked via for/id, ARIA for errors/success, novalidate for custom JS validation, keyboard-focusable elements.
Styling: Shared styles.css with resets, flex/grid, hover/focus states, error/success visuals.

File Structure

portfolio-site/
├── index.html          # Home page (Stage 0 card + nav)
├── contact.html        # Contact form page
├── about.html          # About Me reflective page
├── styles.css          # Shared styles (responsive, accessible)
└── README.md           # This file

Setup and RunningClone/Download: Place files in a folder (e.g., portfolio-site).
Serve Locally:Use VS Code with Live Server extension: Right-click index.html → "Open with Live Server".
Or, use Python: python -m http.server 8000 (navigate to http://localhost:8000).
Or, drag index.html into a browser.

Test Responsiveness: Resize browser or use DevTools device emulation.
Testing: Use data-testids with tools like Jest or Cypress for e2e tests (e.g., form submission).

No build tools or dependencies required—pure vanilla web tech!Development NotesValidation Logic: JS in contact.html uses HTML5 constraints + custom checks. Modular functions for errors/clearing.
Study Resources (Stage 1):Semantic HTML & Accessibility
Form Validation
Form Accessibility
Responsive Media Queries

Future Stages: Prepared for expansion (e.g., more JS interactivity, backend integration).

Acceptance Criteria (Stage 1)Page/Feature
Criteria
Status
Contact Us
All fields/testids present; validation (required, email, min length); success on valid submit.

About Me
All sections/testids; semantic elements (main, section, headings, lists).

General
Semantic HTML; accessible (labels, ARIA, keyboard); responsive (mobile/tablet/desktop); modular code.

ContributingThis is a personal project, but feel free to fork and suggest improvements! Focus on accessibility enhancements or adding animations.LicenseMIT License—free to use, modify, distribute.Built with  by [Your Name] | Last Updated: October 21, 2025 
