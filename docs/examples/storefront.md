---
title: "Storefront mockup: Standard Issue"
layout: raw
---
<style>
  body { margin: 0; font-family: system-ui, sans-serif; color: #17202a; background: #fff; }
  .shop-note { background: #f4f6f8; border-bottom: 1px solid #d8dce0; font-size: .8125rem; padding: .5rem 4vw; color: #4f5963; }
  .shop-note a { color: #b52b16; }
  .shop-nav { display: flex; justify-content: space-between; align-items: center; padding: 1.25rem 4vw; border-bottom: 1px solid #d8dce0; }
  .shop-nav .wordmark { font-weight: 800; letter-spacing: .02em; text-decoration: none; color: #17202a; }
  .shop-nav ul { display: flex; gap: 1.5rem; list-style: none; margin: 0; padding: 0; font-size: .9375rem; }
  .shop-nav a { color: #4f5963; text-decoration: none; }
  .hero { display: grid; grid-template-columns: 1fr 1fr; gap: 2rem; align-items: center; max-width: 72rem; margin: 0 auto; padding: 4rem 4vw 3rem; }
  .hero-photo { aspect-ratio: 4/5; background: #f4f6f8; border: 1px solid #d8dce0; display: flex; align-items: center; justify-content: center; color: #9aa3ab; font-size: .875rem; }
  .hero h1 { font-family: Georgia, serif; font-weight: 400; font-size: clamp(2.25rem, 4vw, 3.5rem); line-height: 1.1; margin: 0 0 1rem; }
  .hero p { font-size: 1.0625rem; line-height: 1.7; margin: 0 0 1.75rem; }
  .price { font-size: 1.25rem; font-weight: 700; margin-bottom: 1.25rem; }
  .cta { display: inline-block; background: #b52b16; color: #fff; text-decoration: none; font-weight: 700; padding: .9rem 2.25rem; border-radius: 2px; }
  .facts { max-width: 72rem; margin: 0 auto; padding: 2.5rem 4vw; border-top: 1px solid #d8dce0; }
  .facts h2, .reassure h2, .faq h2 { font-size: 1.4rem; margin: 0 0 1rem; }
  .facts dl { display: grid; grid-template-columns: max-content 1fr; gap: .5rem 2rem; margin: 0; }
  .facts dt { font-weight: 700; }
  .facts dd { margin: 0; }
  .reassure { max-width: 72rem; margin: 0 auto; padding: 2.5rem 4vw; border-top: 1px solid #d8dce0; display: grid; grid-template-columns: repeat(3, 1fr); gap: 2rem; }
  .reassure h2 { grid-column: 1 / -1; }
  .reassure div { font-size: .9375rem; line-height: 1.6; }
  .reassure strong { display: block; margin-bottom: .25rem; }
  .faq { max-width: 72rem; margin: 0 auto; padding: 2.5rem 4vw; border-top: 1px solid #d8dce0; }
  .faq details { border-bottom: 1px solid #d8dce0; padding: 1rem 0; }
  .faq summary { font-weight: 700; cursor: pointer; }
  .faq p { margin: .75rem 0 0; }
  .shop-footer { border-top: 1px solid #d8dce0; margin-top: 2rem; padding: 2rem 4vw 3rem; font-size: .875rem; color: #4f5963; display: flex; justify-content: space-between; flex-wrap: wrap; gap: 1rem; }
  @media (max-width: 700px) { .hero, .reassure { grid-template-columns: 1fr; } }
</style>

<p class="shop-note"><strong>Teaching example.</strong> Standard Issue is an invented brand created for this book. Nothing on this page is a real product, price, or offer. <a href="{{ '/chapters/07-the-web.html' | relative_url }}">Read the chapter it illustrates →</a></p>

<nav class="shop-nav" aria-label="Store">
  <a class="wordmark" href="#">STANDARD ISSUE</a>
  <ul>
    <li><a href="#facts">The shirt</a></li>
    <li><a href="#reassure">Our promises</a></li>
    <li><a href="#faq">Questions</a></li>
  </ul>
</nav>

<header class="hero">
  <div class="hero-photo" role="img" aria-label="Placeholder for a product photograph of a plain white T-shirt">Product photograph, per the brand guide: single garment, flat daylight, no props</div>
  <div>
    <h1>One good basic. No decisions.</h1>
    <p>A plain white T-shirt in midweight cotton. We make one, we make it properly, and we keep making it. Buy it once or buy it every year — it will be the same shirt.</p>
    <p class="price">$28</p>
    <a class="cta" href="#facts">Add to bag</a>
  </div>
</header>

<section class="facts" id="facts" aria-labelledby="facts-h">
  <h2 id="facts-h">The facts</h2>
  <dl>
    <dt>Fabric</dt><dd>100% cotton, 180 gsm (invented specification for this example)</dd>
    <dt>Fit</dt><dd>Straight cut, crew neck, pre-shrunk</dd>
    <dt>Care</dt><dd>Machine wash cold, line dry or tumble low</dd>
    <dt>Origin</dt><dd>Cut and sewn in Portugal (invented for this example)</dd>
  </dl>
</section>

<section class="reassure" id="reassure" aria-labelledby="reassure-h">
  <h2 id="reassure-h">Our promises</h2>
  <div><strong>Free repairs, forever</strong>Seam splits? Send it back. We would rather fix it than sell you another.</div>
  <div><strong>60-day returns</strong>Wear it. Wash it. If it is not your shirt, it is our problem.</div>
  <div><strong>Same shirt next year</strong>We do not discontinue the basic. That is the whole point of the basic.</div>
</section>

<section class="faq" id="faq" aria-labelledby="faq-h">
  <h2 id="faq-h">Questions people actually ask</h2>
  <details>
    <summary>Is it see-through?</summary>
    <p>It is a midweight knit chosen so it is not. We photograph it over a white surface so you can judge for yourself.</p>
  </details>
  <details>
    <summary>Will the collar hold its shape?</summary>
    <p>The collar is a ribbed knit with a taped seam. It holds up to regular washing; line drying helps it last longer.</p>
  </details>
  <details>
    <summary>Why only one product?</summary>
    <p>Because deciding is work, and we would rather do it once, well, on your behalf.</p>
  </details>
</section>

<footer class="shop-footer">
  <span>STANDARD ISSUE — an invented brand for teaching.</span>
  <span>Contact · Shipping · Returns · Privacy</span>
</footer>
