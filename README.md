# Nimbus Coworking

Website for Nimbus Coworking, a shared workspace in the centre of town. Private
offices, open desks and meeting rooms — book by the day or by the year.

**Live site: https://kenza12.github.io/nimbus-coworking/**

## Pages

| Page | File | What it contains |
|---|---|---|
| Home | `index.html` | What Nimbus is, what is included, and how to book a tour |
| Spaces | `spaces.html` | The three kinds of workspace, and the community side of Nimbus |
| Pricing | `pricing.html` | Plans for individuals and for teams |
| Contact | `contact.html` | Contact form, address, opening hours and directions |

## Built with

Semantic HTML and vanilla CSS. No framework, no build step, no JavaScript.
Layouts use Flexbox, and Font Awesome provides the icons.

## Project structure

```
nimbus-coworking/
├── index.html
├── spaces.html
├── pricing.html
├── contact.html
└── assets/
    ├── css/
    │   ├── main.css          shared: variables, header, footer, buttons
    │   └── pages/
    │       ├── home.css
    │       ├── spaces.css
    │       ├── pricing.css
    │       └── contact.css
    ├── fonts/                Roboto
    └── images/
```

`main.css` holds everything shared between pages: the colour variables, the
header, the navigation, the footer and the page intro banner. Each page then
loads its own stylesheet for what is specific to it.

## Colours and typography

| Variable | Value | Used for |
|---|---|---|
| `--color-dark` | `#1F2937` | Header, hero and footer background |
| `--color-light` | `#F9FAF8` | Main text on dark backgrounds, logo |
| `--color-secondary` | `#E5E7EB` | Secondary text, quote section background |
| `--color-accent` | `#3882F6` | Buttons, borders, call to action |

Roboto is loaded locally with `@font-face`: 48px extra-bold for the hero title,
36px extra-bold for section headings, 24px for the logo, 18px for body text.

## Responsive design

The site adapts to mobile (375px), tablet (768px) and desktop (1200px and above).

## Team workflow

`main` holds the stable version, `dev` is the integration branch. Each task gets
its own `feat/*` or `fix/*` branch, merged into `dev` through a pull request.
`dev` is merged into `main` once it is stable.