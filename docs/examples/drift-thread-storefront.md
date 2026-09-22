---
title: "Storefront mockup: Drift & Thread"
layout: raw
---
<style>
  body { margin: 0; font-family: system-ui, sans-serif; color: #2e3b2f; background: #faf6ef; }
  .shop-note { background: #f4f6f8; border-bottom: 1px solid #d8dce0; font-size: .8125rem; padding: .5rem 4vw; color: #4f5963; }
  .shop-note a { color: #b52b16; }
  .shop-nav { display: flex; justify-content: space-between; align-items: center; padding: 1.25rem 4vw; border-bottom: 1px solid #e2d9c8; }
  .shop-nav .wordmark { font-family: Georgia, serif; font-style: italic; font-size: 1.25rem; text-decoration: none; color: #2e3b2f; }
  .shop-nav ul { display: flex; gap: 1.5rem; list-style: none; margin: 0; padding: 0; font-size: .9375rem; }
  .shop-nav a { color: #5c6b5d; text-decoration: none; }
  .hero { display: grid; grid-template-columns: 1.15fr 1fr; gap: 2.5rem; align-items: center; max-width: 72rem; margin: 0 auto; padding: 4rem 4vw 3rem; }
  .hero-photo { aspect-ratio: 4/3; background: linear-gradient(160deg, #e8dfce, #cfd8dc); border: none; display: flex; align-items: center; justify-content: center; color: #7d8a7e; font-size: .875rem; text-align: center; padding: 1rem; }
  .hero h1 { font-family: Georgia, serif; font-weight: 400; font-size: clamp(2.25rem, 4vw, 3.5rem); line-height: 1.1; margin: 0 0 1rem; }
  .hero p { font-size: 1.0625rem; line-height: 1.7; margin: 0 0 1.75rem; }
  .price { font-size: 1.25rem; font-weight: 700; margin-bottom: 1.25rem; }
  .cta { display: inline-block; background: #c2703e; color: #fff; text-decoration: none; font-weight: 700; padding: .9rem 2.25rem; border-radius: 999px; }
  .facts { max-width: 72rem; margin: 0 auto; padding: 2.5rem 4vw; border-top: 1px solid #e2d9c8; }
  .facts h2, .reassure h2, .faq h2 { font-family: Georgia, serif; font-weight: 400; font-size: 1.5rem; margin: 0 0 1rem; }
  .facts dl { display: grid; grid-template-columns: max-content 1fr; gap: .5rem 2rem; margin: 0; }
  .facts dt { font-weight: 700; }
  .facts dd { margin: 0; }
  .reassure { max-width: 72rem; margin: 0 auto; padding: 2.5rem 4vw; border-top: 1px solid #e2d9c8; display: grid; grid-template-columns: repeat(3, 1fr); gap: 2rem; }
  .reassure h2 { grid-column: 1 / -1; }
  .reassure div { font-size: .9375rem; line-height: 1.6; }
  .reassure strong { display: block; margin-bottom: .25rem; }
  .faq { max-width: 72rem; margin: 0 auto; padding: 2.5rem 4vw; border-top: 1px solid #e2d9c8; }
  .faq details { border-bottom: 1px solid #e2d9c8; padding: 1rem 0; }
  .faq summary { font-weight: 700; cursor: pointer; }
  .faq p { margin: .75rem 0 0; }
  .shop-footer { border-top: 1px solid #e2d9c8; margin-top: 2rem; padding: 2rem 4vw 3rem; font-size: .875rem; color: #5c6b5d; display: flex; justify-content: space-between; flex-wrap: wrap; gap: 1rem; }
  @media (max-width: 700px) { .hero, .reassure { grid-template-columns: 1fr; } }
</style>

<p class="shop-note"><strong>Teaching example.</strong> Drift &amp; Thread is an invented brand created for this book — the same fictional shirt as the Standard Issue mockup, told differently. <a href="{{ '/chapters/07-the-web.html' | relative_url }}">Read the chapter it illustrates →</a></p>

<nav class="shop-nav" aria-label="Store">
  <a class="wordmark" href="#">Drift &amp; Thread</a>
  <ul>
    <li><a href="#facts">The shirt</a></li>
    <li><a href="#reassure">Field notes</a></li>
    <li><a href="#faq">Questions</a></li>
  </ul>
</nav>

<header class="hero">
  <div class="hero-photo" role="img" aria-label="Placeholder for a product photograph of a white T-shirt drying over a chair beside a train window">Product photograph, per the brand guide: the shirt in use, warm light, one bag beside it</div>
  <div>
    <h1>The shirt that's already packed.</h1>
    <p>Some shirts live in drawers. This one lives in your bag. Midweight cotton that handles a night bus and a morning meeting, washes clean in a sink, and dries by the time the coffee's ready.</p>
    <p class="price">$28</p>
    <a class="cta" href="#facts">Pack one</a>
  </div>
</header>

<section class="facts" id="facts" aria-labelledby="facts-h">
  <h2 id="facts-h">The label, because you'll check</h2>
  <dl>
    <dt>Fabric</dt><dd>100% cotton, 180 gsm (invented specification for this example)</dd>
    <dt>Fit</dt><dd>Straight cut, crew neck, pre-shrunk</dd>
    <dt>Care</dt><dd>Machine wash cold, line dry or tumble low — sink-tested</dd>
    <dt>Origin</dt><dd>Cut and sewn in Portugal (invented for this example)</dd>
  </dl>
</section>

<section class="reassure" id="reassure" aria-labelledby="reassure-h">
  <h2 id="reassure-h">Field notes</h2>
  <div><strong>Dries overnight</strong>Washed at 10pm in a Lisbon sink, worn at 7am. We time these things so you don't have to.</div>
  <div><strong>60-day returns, from anywhere</strong>Changed your mind in another time zone? We'll sort it out when you land.</div>
  <div><strong>Repairs travel too</strong>A split seam shouldn't end a trip. Send it back; we'll fix it and cover the postage.</div>
</section>

<section class="faq" id="faq" aria-labelledby="faq-h">
  <h2 id="faq-h">Questions from the road</h2>
  <details>
    <summary>Does white really work for travel?</summary>
    <p>Better than you'd think. It shows dirt honestly, washes hot when it must, and matches everything you didn't pack.</p>
  </details>
  <details>
    <summary>Is it heavy in a bag?</summary>
    <p>At 180 gsm it's the middle ground: opaque in daylight, light enough to forget, quick to dry.</p>
  </details>
  <details>
    <summary>Will it smell after a long travel day?</summary>
    <p>Cotton breathes better than synthetics on a long day, and a sink wash resets it completely. Pack two and you'll never think about it again.</p>
  </details>
</section>

<footer class="shop-footer">
  <span>Drift &amp; Thread — an invented brand for teaching.</span>
  <span>Contact · Shipping · Returns · Privacy</span>
</footer>
