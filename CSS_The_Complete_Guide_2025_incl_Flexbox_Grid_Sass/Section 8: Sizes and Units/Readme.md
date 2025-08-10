Here’s a compact summary table for your updated shared.css:
| Selector | Target / Scope | Key Declarations | What it does |
| ------------------------------------------------------------- | --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `*` | All elements | `box-sizing: border-box` | Includes padding/border in element dimensions. |
| `body` | Page root | `font-family: "Montserrat"`, `margin: 0` | Global font, removes default margin. |
| `.backdrop` | Full-screen overlay | `position: fixed; display: none; top/left: 0; z-index: 100; width: 100vw; height: 100vh; background: rgba(0,0,0,.5)` | Hidden modal backdrop; covers whole viewport when shown. |
| `.main-header` | Header bar (fixed) | `position: fixed; top: 0; left: 0; width: 100%; background: #2ddf5c; padding: .5rem 1rem; z-index: 1` | Sticky green header pinned to top. |
| `.main-header > div` | Direct child wrappers | `display: inline-block; vertical-align: middle` | Aligns brand/nav side-by-side and centered. |
| `.main-header__brand` | Brand link | `color: #0e4f1f; text-decoration: none; font-weight: bold; font-size: 1.5rem; height: 1.5rem; display: inline-block` | Bold dark-green brand; sets logo text/box height. |
| `.main-header__brand img` | Brand image | `height: 100%` | Logo image fills the brand box height. |
| `.main-nav` | Nav container | `display: inline-block; text-align: right; width: calc(100% - 74px); vertical-align: middle` | Sits next to brand; right-aligns links; fills remaining width. |
| `.main-nav__items` | Nav list (`ul`) | `margin: 0; padding: 0; list-style: none` | Removes default spacing/bullets. |
| `.main-nav__item` | Nav item (`li`) | `display: inline-block; margin: 0 1rem` | Horizontal menu with spacing. |
| `.main-nav__item a` | Nav links | `text-decoration: none; color: #0e4f1f; font-weight: bold; padding: .2rem 0` | Bold dark-green links without underline. |
| `.main-nav__item a:hover, .main-nav__item a:active` | Link hover/active | `color: white; border-bottom: 5px solid white` | Turns link white with thick underline on interaction. |
| `.main-nav__item--cta a` | CTA link | `color: white; background: #ff1b68; padding: .5rem 1rem; border-radius: 8px` | Pink rounded CTA button with white text. |
| `.main-nav__item--cta a:hover, .main-nav__item--cta a:active` | CTA hover/active | `color: #ff1b68; background: white; border: none` | Inverts CTA colors on interaction. |
| `.main-footer` | Footer bar | `background: black; padding: 2rem; margin-top: 3rem` | Spacious black footer separated from content. |
| `.main-footer__links` | Footer list (`ul`) | `list-style: none; margin: 0; padding: 0; text-align: center` | Centered, bullet-less footer links. |
| `.main-footer__link` | Footer item (`li`) | `display: inline-block; margin: 0 1rem` | Horizontal footer menu with spacing. |
| `.main-footer__link a` | Footer anchors | `color: white; text-decoration: none` | White links without underline. |
| `.main-footer__link a:hover, .main-footer__link a:active` | Footer link states | `color: #ccc` | Light gray on hover/active. |
| `.button` | Reusable button | `background: #0e4f1f; color: white; font: inherit; border: 1.5px solid #0e4f1f; padding: .5rem; border-radius: 8px; font-weight: bold; cursor: pointer` | Dark-green rounded button with matching border. |
| `.button:hover, .button:active` | Button states | `background: white; color: #0e4f1f` | Inverts colors on interaction. |
| `.button:focus` | Button focus | `outline: none` | Removes default focus ring (consider adding a custom visible focus for accessibility). |

Here’s a clean summary table for your updated main.css:
| Selector | Target / Scope | Key Declarations | What it does |
| --------------------------------- | ----------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `#product-overview` | Hero/intro banner | `background: linear-gradient(...) , url("images/freedom.jpg") left 10% bottom 70% / cover no-repeat border-box, #ff1b68; width: 100vw; height: 33vh; margin-top: 2.75rem; position: relative` | Multi-layer background: a semi-transparent gradient **over** the image, with a pink fallback color. Image is sized to **cover**, positioned 10% from left / 70% from bottom, no repeat. Full viewport width, 33% viewport height, offset from fixed header; `position: relative` anchors the inner absolute H1. |
| `.section-title` | Section headings | `color: #2ddf5c; text-align: center` | Green, centered section titles. |
| `#product-overview h1` | Hero title | `color: white; font-family: "Anton", sans-serif; position: absolute; bottom: 5%; left: 3%` | White Anton headline positioned near bottom-left of the hero. |
| `.plan__list` | Plans wrapper | `width: 80%; margin: auto; text-align: center` | Centers the plan cards and their contents. |
| `.plan` | Plan card (default) | `background: #d5ffdc; text-align: center; padding: 1rem; margin: 0.5rem; display: inline-block; width: 30%; vertical-align: middle` | Green-tinted cards laid out \~3 across with spacing. |
| `.plan--highlighted` | Featured plan | `background: #19b84c; color: white; box-shadow: 2px 2px 2px 2px rgba(0,0,0,.5)` | Darker green featured card, white text, shadow emphasis. |
| `.plan__annotation` | Plan badge | `background: white; color: #19b84c; padding: .5rem; box-shadow: ...; border-radius: 8px` | White pill/tag badge with green text and shadow. |
| `.plan__title` | Plan heading | `color: #0e4f1f` | Dark-green titles. |
| `.plan__price` | Plan price | `color: #858585` | Neutral gray price text. |
| `.plan--highlighted .plan__title` | Title in featured card | `color: white` | Title flips to white for contrast. |
| `.plan--highlighted .plan__price` | Price in featured card | `color: #0e4f1f` | Price turns dark green for contrast. |
| `.plan__features` | Feature list (`ul`) | `list-style: none; margin: 0; padding: 0` | Removes bullets and default spacing. |
| `.plan__feature` | Feature item (`li`) | `margin: .5rem 0` | Vertical spacing between features. |
| `#key-features` | Features band | `background: #ff1b68; margin-top: 5rem; padding: 1rem` | Pink highlight section with extra top spacing. |
| `#key-features .section-title` | Title inside band | `color: white; margin: 2rem` | White, well-spaced heading. |
| `.key-feature__list` | Feature items container | `list-style: none; margin: 0; padding: 0; text-align: center` | Centers feature blocks; no bullets. |
| `.key-feature` | Single feature block | `display: inline-block; width: 30%; vertical-align: top` | \~3-column layout of features. |
| `.key-feature__image` | Feature icon circle | `background: #ffcede; width: 128px; height: 128px; border: 2px solid #424242; border-radius: 50%; margin: auto; padding: 1.5rem` | Centered pink circle (avatar/badge) with inner padding. |
| `.key-feature__description` | Feature caption | `text-align: center; font-weight: bold; color: white; font-size: 1.2rem` | Bold, white, centered description text. |
