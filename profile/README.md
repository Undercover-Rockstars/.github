<p align="center">
  <img src="https://raw.githubusercontent.com/Undercover-Rockstars/.github/main/assets/org-banner.png" alt="Undercover Rockstars — everyone has a rockstar undercover." width="100%">
</p>

<p align="center">
  <a href="https://undercoverrockstars.com"><img src="https://img.shields.io/badge/UNDERCOVERROCKSTARS.COM-LIVE-EF3B2C?style=for-the-badge&labelColor=0A0A0B" alt="undercoverrockstars.com"></a>
  <img src="https://img.shields.io/badge/DROP%2001-NOT%20YET%20SELLING-ECEBE6?style=for-the-badge&labelColor=0A0A0B" alt="Drop 01: not yet selling">
  <a href="https://factory0.ventures"><img src="https://img.shields.io/badge/FZ--002-FACTORY%20ZERO-FF5A36?style=for-the-badge&labelColor=0A0A0B" alt="FZ-002, a Factory Zero venture"></a>
</p>

<p align="center">
  <sub>
    <a href="https://undercoverrockstars.com">Site</a> &nbsp;·&nbsp;
    <a href="https://undercoverrockstars.com/collection/">The collection</a> &nbsp;·&nbsp;
    <a href="https://undercoverrockstars.com/thesis/">Thesis</a> &nbsp;·&nbsp;
    <a href="https://undercoverrockstars.com/waitlist/">Waitlist</a> &nbsp;·&nbsp;
    <a href="https://undercoverrockstars.com/catalogue.json">catalogue.json</a> &nbsp;·&nbsp;
    <a href="https://undercoverrockstars.com/llms.txt">llms.txt</a>
  </sub>
</p>

---

## One pattern, cut twice.

Undercover Rockstars makes clothing for people who live two lives in one day.

Every piece comes as a **matched pair**: one for the meeting, one for what comes
after. The same pattern is cut twice, once for the day and once for the night,
so the fit never changes when the room does. You are not a different person at
9am and at 11pm — you should not have to dress like one.

> **Everyone has a rockstar undercover.**

**Drop 01** is eight pairs — sixteen garments — cut in **Bali**.

---

## How the house works

| | |
| :--- | :--- |
| **Pairs, not pieces** | Eight pairs in Drop 01. Day and night share a pattern, not a compromise |
| **Two fits** | Standard, or **made to measure** at +30% |
| **Cut in** | Bali, Indonesia |
| **Prices** | USD across the site |
| **The tag** | Each garment carries an NFC tag meant to prove authenticity and let a finder reach the owner |

---

## Status: nothing is on sale yet

We would rather say this plainly than let a beautiful landing page imply
otherwise.

- **Drop 01 has not shipped.** No garment exists to buy today, and there is no
  checkout on the site — the product pages are `PreOrder`, and there is no card
  field anywhere.
- **The waitlist sells a $9 place** in the queue, credited against your first
  pair and **not refundable**. It only takes payment once the processor is
  connected; until then it says so rather than pretending.
- **The NFC tag has nothing to tap yet.** The registry and the finder-to-owner
  relay are not built, and every surface that mentions the tag hedges on that.

---

## The fitting room

A phone-based body scan, so a made-to-measure order does not need a tailor in
the room. Open [`/fit/`](https://undercoverrockstars.com/fit/) on a phone, or
hit "Try it on" on desktop and scan the QR.

It runs **entirely on the device**. The pose model is vendored rather than
pulled from a CDN, and it loads only after you consent, so simply viewing the
page costs nothing. It measures the silhouette of the segmentation mask, not
landmark coordinates, and turns front width and side depth into circumference.

**Your photos never leave the phone.** Nothing is uploaded, and accuracy against
a real tape measure is still unproven — so there is a tape-check mode in the app
and a human confirmation step before anything is cut.

---

## Readable by machines

| Surface | Purpose |
| :--- | :--- |
| [`catalogue.json`](https://undercoverrockstars.com/catalogue.json) | Every pair, both fit prices, shipping, the tag and the waitlist, with `purchasable` flags. Served `Access-Control-Allow-Origin: *` |
| [`llms.txt`](https://undercoverrockstars.com/llms.txt) | Plain-text brief that leads with what is and is not for sale |

Please carry the not-yet-selling status with any claim about the drop.

---

## Repositories

| Repo | What it is |
| :--- | :--- |
| [**website**](https://github.com/Undercover-Rockstars/website) | [undercoverrockstars.com](https://undercoverrockstars.com) and the `/fit/` PWA. Static HTML, no build step, dependencies vendored, no CDN |
| **.github** | This page, the star and the banner |

<p align="center">
  <br>
  <sub>
    <b>FZ-002</b> &nbsp;·&nbsp; a <a href="https://factory0.ventures">Factory Zero</a> venture
  </sub>
</p>
