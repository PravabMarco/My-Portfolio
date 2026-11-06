# Personal Portfolio

A single-page, 3D animated portfolio for a BCA student based in Kathmandu, Nepal. The whole site is one file, `index.html`, with no build step.

## Features

- 3D hero: a fan of glass cards drawn with three.js, on a tilted screen that lies flat as you scroll.
- Skills doors: three arched doors that open on hover or tap to show the skill list. A button opens or closes all of them.
- Journey: a pinned scroll section that counts back from semester 8 to 2022.
- Work: Bike Parts E-commerce, Fitness web app, College Event Management System and Vex Scales.
- GitHub repository list and contact section.
- Glass navigation bar whose text colour follows the section behind it.
- Colours taken only from the Benjamin Moore Simply White OC-117 palette.
- Respects the reduced motion setting. Works at phone width.

## Run it

1. Put `index.html` in a folder.
2. Open it in a browser. An internet connection is needed for the libraries and fonts below.

To publish it, upload `index.html` to GitHub Pages or any static host. For a repository named `<username>.github.io`, put the file in the root of the repository.

## Edit it

| What | Where in `index.html` |
| --- | --- |
| Name | Search for the name in the title, header logo, hero heading and footer |
| Email | `CONFIG.email` in the script at the end of the file |
| LinkedIn link | The "Message on LinkedIn" link in the contact section |
| Project text | The `<article class="card">` blocks in the Work section |
| GitHub repositories | The `<div class="repos">` block in the Work section |
| Skills | The three `<article class="door">` blocks in the Skills section |
| Semesters | The `<div class="step">` blocks in the Journey section |
| Colours | The variables at the top of the `<style>` block (`--simply`, `--vogue`, `--navy` and so on) |

## Colour palette

| Name | Hex |
| --- | --- |
| Simply White | `#eae9e1` |
| Dove White | `#eeeee4` |
| Chantilly Lace | `#f4f5f0` |
| Balboa Mist | `#dad6cb` |
| Revere Pewter | `#cbc5b8` |
| Boothbay Gray | `#a9b1ae` |
| Hale Navy | `#434b56` |
| Vintage Vogue | `#596052` |

## Built with

- HTML, CSS and JavaScript, with no framework
- [three.js](https://threejs.org/) r128 (3D hero)
- [GSAP](https://gsap.com/) 3.12.5 and ScrollTrigger (scroll animation)
- [Google Fonts](https://fonts.google.com/): Outfit and DM Sans

The libraries load from cdnjs and the fonts from Google Fonts.

## Ideas taken from

react-three-fiber, liquid-glass-js, threeui.com, tasteskill.dev, demos.gsap.com and 21st.dev.

## Browser support

Current versions of Chrome, Edge, Firefox and Safari. If WebGL is not available, the hero shows a plain gradient shape instead of the 3D cards.
