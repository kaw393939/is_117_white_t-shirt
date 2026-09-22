---
title: "Storefront mockup: Blank Canvas Co."
layout: raw
---
<style>
  body { margin: 0; font-family: system-ui, sans-serif; color: #1a1a1a; background: #fff; }
  .shop-note { background: #f4f6f8; border-bottom: 1px solid #d8dce0; font-size: .8125rem; padding: .5rem 4vw; color: #4f5963; }
  .shop-note a { color: #b52b16; }
  .shop-nav { display: flex; justify-content: space-between; align-items: center; padding: 1.25rem 4vw; background: #fff200; border-bottom: 3px solid #1a1a1a; }
  .shop-nav .wordmark { font-weight: 900; letter-spacing: -.02em; text-transform: uppercase; text-decoration: none; color: #1a1a1a; transform: rotate(-1.5deg); display: inline-block; }
  .shop-nav ul { display: flex; gap: 1.5rem; list-style: none; margin: 0; padding: 0; font-size: .9375rem; font-weight: 700; }
  .shop-nav a { color: #1a1a1a; text-decoration: none; }
  .hero { display: grid; grid-template-columns: 1fr 1.1fr; gap: 2.5rem; align-items: center; max-width: 72rem; margin: 0 auto; padding: 4rem 4vw 3rem; }
  .hero-photo { aspect-ratio: 1; background: #3ec1f3; border: 3px solid #1a1a1a; box-shadow: 8px 8px 0 #ff4fa3; display: flex; align-items: center; justify-content: center; color: #1a1a1a; font-size: .875rem; text-align: center; padding: 1rem; transform: rotate(1deg); font-weight: 700; }
  .hero h1 { font-weight: 900; text-transform: uppercase; letter-spacing: -.03em; font-size: clamp(2.25rem, 4.5vw, 3.75rem); line-height: 1; margin: 0 0 1rem; }
  .hero h1 em { background: #fff200; padding: 0 .15em; font-style: normal; }
  .hero p { font-size: 1.0625rem; line-height: 1.7; margin: 0 0 1.75rem; }
  .price { font-size: 1.5rem; font-weight: 900; margin-bottom: 1.25rem; }
  .price small { font-weight: 400; font-size: .875rem; }
  .cta { display: inline-block; background: #ff4fa3; color: #fff; text-decoration: none; font-weight: 900; text-transform: uppercase; letter-spacing: .02em; padding: .9rem 2.25rem; border: 3px solid #1a1a1a; box-shadow: 5px 5px 0 #1a1a1a; }
  .facts { max-width: 72rem; margin: 0 auto; padding: 2.5rem 4vw; border-top: 3px solid #1a1a1a; }
  .facts h2, .reassure h2, .faq h2 { font-size: 1.5rem; font-weight: 900; text-transform: uppercase; letter-spacing: -.01em; margin: 0 0 1rem; }
  .facts dl { display: grid; grid-template-columns: max-content 1fr; gap: .5rem 2rem; margin: 0; }
  .facts dt { font-weight: 700; }
  .facts dd { margin: 0; }
  .reassure { max-width: 72rem; margin: 0 auto; padding: 2.5rem 4vw; border-top: 3px solid #1a1a1a; display: grid; grid-template-columns: repeat(3, 1fr); gap: 2rem; }
  .reassure h2 { grid-column: 1 / -1; }
  .reassure div { font-size: .9375rem; line-height: 1.6; border: 2px solid #1a1a1a; padding: 1rem; }
  .reassure div:nth-child(2) { background: #fff200; transform: rotate(-1deg); }
  .reassure div:nth-child(3) { background: #3ec1f3; }
  .reassure div:nth-child(4) { background: #fff; transform: rotate(1deg); }
  .reassure strong { display: block; margin-bottom: .25rem; }
  .faq { max-width: 72rem; margin: 0 auto; padding: 2.5rem 4vw; border-top: 3px solid #1a1a1a; }
  .faq details { border-bottom: 2px solid #1a1a1a; padding: 1rem 0; }
  .faq summary { font-weight: 700; cursor: pointer; }
  .faq p { margin: .75rem 0 0; }
  .shop-footer { background: #1a1a1a; color: #fff; margin-top: 2rem; padding: 2rem 4vw 3rem; font-size: .875rem; display: flex; justify-content: space-between; flex-wrap: wrap; gap: 1rem; }
  @media (max-width: 700px) { .hero, .reassure { grid-template-columns: 1fr; } }
</style>

<p class="shop-note"><strong>Teaching example.</strong> Blank Canvas Co. is an invented brand created for this book — the same fictional shirt as the other two mockups, with the volume turned up. <a href="{{ '/chapters/07-the-web.html' | relative_url }}">Read the chapter it illustrates →</a></p>

<nav class="shop-nav" aria-label="Store">
  <a class="wordmark" href="#">Blank Canvas Co.</a>
  <ul>
    <li><a href="#facts">The boring truth</a></li>
    <li><a href="#reassure">Promises</a></li>
    <li><a href="#faq">Interrogation</a></li>
  </ul>
</nav>

<header class="hero">
  <div class="hero-photo" role="img" aria-label="Placeholder for a product photograph of a white T-shirt presented on a velvet pillow like jewelry">Product photograph, per the brand guide: the shirt on a velvet pillow, presented like jewelry</div>
  <div>
    <h1>It's a <em>white T-shirt.</em> We've made peace with that.</h1>
    <p>Behold: a shirt. White. Short sleeves. A hole for your head — arguably our best feature. It will not change your life. It will cover your torso competently and without ceremony.</p>
    <p class="price">$28 <small>(an honestly normal price)</small></p>
    <a class="cta" href="#facts">Fine, I'll take one</a>
  </div>
</header>

<section class="facts" id="facts" aria-labelledby="facts-h">
  <h2 id="facts-h">The boring truth</h2>
  <dl>
    <dt>Fabric</dt><dd>100% cotton, 180 gsm — a real number we are proud of (invented for this example)</dd>
    <dt>Fit</dt><dd>Straight cut, crew neck, pre-shrunk</dd>
    <dt>Care</dt><dd>Machine wash cold. It has been through enough.</dd>
    <dt>Origin</dt><dd>Cut and sewn in Portugal (invented for this example)</dd>
  </dl>
</section>

<section class="reassure" id="reassure" aria-labelledby="reassure-h">
  <h2 id="reassure-h">Promises (legally distinct from jokes)</h2>
  <div><strong>Free repairs, forever</strong>Tear it living your life. We'll fix it and pretend it never happened.</div>
  <div><strong>60-day returns</strong>Don't love it? Send it back. We'll only be a little hurt.</div>
  <div><strong>No fake countdown timers</strong>This shirt will still exist tomorrow. That is a business model, apparently.</div>
</section>

<section class="faq" id="faq" aria-labelledby="faq-h">
  <h2 id="faq-h">Interrogation</h2>
  <details>
    <summary>Is this a joke?</summary>
    <p>The copy, yes. The shirt, no. 100% cotton, 180 gsm, sewn by professionals who did not find any of this funny.</p>
  </details>
  <details>
    <summary>Is it see-through?</summary>
    <p>No. We tested this extensively, in a well-lit room, with a witness.</p>
  </details>
  <details>
    <summary>Why should I buy a plain white tee from a brand with jokes?</summary>
    <p>Because the jokes are free and the shirt is serious. You're paying $28 for cotton; the entertainment is included at no charge.</p>
  </details>
</section>

<footer class="shop-footer">
  <span>Blank Canvas Co. — an invented brand for teaching.</span>
  <span>Contact · Shipping · Returns · Privacy</span>
</footer>
