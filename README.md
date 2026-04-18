<p align="center">
  <img src="https://img.shields.io/badge/HTML-5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS-3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/Zero_Build-Zero_Deps-22C55E?style=for-the-badge" alt="Zero build" />
  <img src="https://img.shields.io/badge/Studio_Builder-Ready-8B5CF6?style=for-the-badge" alt="Studio Builder Ready" />
  <img src="https://img.shields.io/badge/AI-Ready-F59E0B?style=for-the-badge" alt="AI Ready" />
</p>

<h1 align="center">VA Studio HTML Starter — Registration</h1>

<p align="center">
  <strong>A split-layout account creation page with brand panel, OAuth buttons, and password strength meter.</strong>
</p>

<p align="center">
  Left-side marketing panel with testimonial and trust badges, right-side registration form<br/>
  with Google / GitHub OAuth, password visibility toggle, and a polished success state.
</p>

<p align="center">
  <a href="#quick-start">Quick Start</a> &bull;
  <a href="#sections">Sections</a> &bull;
  <a href="#studio-builder-integration">Studio Integration</a> &bull;
  <a href="#customizing">Customizing</a>
</p>

---

## Quick Start

```bash
python -m http.server 8000
# or
npx serve .
```

Open [http://localhost:8000](http://localhost:8000).

## Sections

- **Brand panel (left)** — full-bleed background image with dark/indigo gradient overlay, brand mark, headline, lead, embedded testimonial with avatar, trust row (SOC 2 / GDPR / SLA)
- **Form panel (right)** — header with brand mark (mobile-only), title, subtitle
- **OAuth row** — "Continue with Google" and "Continue with GitHub" buttons, real SVG brand marks
- **Divider** — "or continue with email"
- **Form fields** — first/last name, work email + hint, password with visibility toggle and strength bars, company, role select
- **Terms checkbox** — with links to Terms / Privacy
- **Primary submit** — slate-900 CTA
- **Success state** — appears on submit with check icon and inbox-verification copy

## Studio Builder Integration

- Form controls have predictable IDs (`#first`, `#last`, `#email`, `#password`, `#company`, `#role`) for Studio bindings
- OAuth buttons are type-safe and ready to swap for Studio auth providers
- Password strength bars are pure CSS — Studio can drive them via a dynamic class (`.strength-bar.active`)
- Success state is toggled by the `hidden` attribute — easy to control from Studio event handlers

## Tech Stack

| Layer | Technology |
|-------|-----------|
| **Markup** | HTML5 forms with proper autocomplete hints |
| **Styling** | CSS3, split grid layout, mobile responsive |
| **Fonts** | Inter + Playfair Display (Google Fonts) |
| **Images** | Unsplash (brand-panel background), pravatar (testimonial avatar) |
| **Icons** | Inline SVG (Google, GitHub, eye toggle, check) |

## Project Structure

```
va_studio_html_starter_registration/
├── index.html      # Split registration page
├── styles.css      # Panel layout, form controls, responsive breakpoints
└── README.md
```

## Customizing

- **Brand panel image:** swap the Unsplash URL inside `.brand-bg` background-image
- **Testimonial:** edit the `<blockquote>` and pravatar URL inside `.testimonial`
- **OAuth providers:** duplicate the `.btn-oauth` pattern for more SSO options
- **Roles:** edit the `<option>` list inside `#role`
- **Palette:** CSS vars at top of `styles.css` — `--accent` drives focus rings and links

## License

MIT

---

<p align="center">
  Part of the <strong>VA Studio</strong> starter family · Built for rapid prototyping with an AI copilot.
</p>
