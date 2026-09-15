---
name: Lim Zi Chao GitHub Profile
description: A restrained editorial portfolio in forest, ivory, and muted gold.
colors:
  forest: "#193e34"
  ivory: "#f4f1e8"
typography:
  display:
    fontFamily: "Baskerville, 'Palatino Linotype', Georgia, serif"
  project-title:
    fontFamily: "Baskerville, 'Palatino Linotype', Georgia, serif"
    fontSize: "66px"
    letterSpacing: "-1px"
---

# Design System: Lim Zi Chao GitHub Profile

## Overview

**Creative North Star: "The Editorial Portfolio"**

Restrained serif artwork gives the profile a recognizable identity; native
GitHub text carries the evidence and actions. The visual system is static,
flat, and deliberately small.

**Key Characteristics:**

- Forest and ivory anchors with quiet geometric accents.
- Full-width artwork followed by readable native descriptions.
- Repository-hosted SVGs; no application CSS or JavaScript.

## Colors

Forest supplies the recurring dark field and lettering; ivory supplies the
masthead field and reversed lettering. Muted gold geometry and pale sage
differentiate the artwork. Their fixed, asset-local colors live in
`assets/*.svg`; they are not page-theme tokens.

GitHub owns body, link, divider, and background colors in its light and dark
themes. SVG palettes do not change with the host theme.

## Typography

The SVG display stack uses locally available serif fonts with explicit
fallbacks; no font is downloaded or embedded. The masthead name is larger than
the shared project-title role, with a Georgia serif subtitle. SVG font sizes
are intrinsic drawing units, not guaranteed on-screen CSS sizes.

GitHub owns body text, Markdown headings, bold emphasis, and `<sub>` technology
lines. There is no custom production body-font or heading-size rule.

## Layout

A single reading column alternates images, descriptions, and text links.
All images are 960 units wide: the masthead is 300 units high and project
banners are 150. GitHub constrains them to the available column width; their
viewBoxes scale proportionally without breakpoint-specific rearrangement.

Project titles share a left inset of 40 drawing units; geometric illustrations
occupy the right-hand side. Native paragraph spacing and explicit `<br>` gaps
separate major blocks. `&nbsp;` keeps compact separators apart in link and
technology rows. The final Markdown rule separates the footer.

## Elevation & Depth

Flat fills, fine linework, and contrasting fields provide separation. The
shipped artwork has no shadows, gradients, animation, or hover effects.

## Shapes

Square-edged rectangular image fields contain precise outlined geometry:
intersecting forms in the masthead, orbital forms for Plutus, and an angular
conversation/check symbol for Green Chonk. Geometry is illustration, not UI.

## Components

The masthead is a static identity image. Project banners are native image
links, followed by selectable project context, descriptions, technologies,
and explicitly labeled actions. Standard Markdown links supply all navigation;
GitHub controls their hover and keyboard-focus presentation.

Each image has Markdown alt text and SVG title/description metadata. Essential
project evidence and destinations remain in native text outside the images.
Preserve that duplication: small-screen proportional scaling reduces artwork
text size, and SVG metadata support varies between image consumers.

## Do's and Don'ts

- Do preserve full-width proportional SVG scaling and explicit serif fallbacks.
- Do pair visual project headers with native descriptions and meaningful links.
- Don't encode essential project evidence only inside artwork.
- Don't treat GitHub theme styling or the ignored local review preview as custom production CSS.
