---
layout: default
title: "Newsletter — Yogi & Linga"
permalink: /newsletter/
description: "Get independent sexual wellness reviews, buying guides, and science reads — delivered weekly. No spam. Unsubscribe anytime."
---

<div class="article-header">
  <p class="article-category">FREE NEWSLETTER</p>
  <h1 class="article-title">Honest reviews.<br>No noise. No spam.</h1>
  <p style="color: var(--cream-dim); font-size: 1rem; line-height: 1.8; max-width: 520px; margin: 1rem auto 0;">
    Join readers who get our weekly picks — top-tested products, science reads, and buying advice you can actually use.
  </p>
</div>

<div style="max-width: 580px; margin: 0 auto; padding: 0 2rem 5rem;">

  <div style="background: rgba(255,255,255,0.02); border: 0.5px solid var(--border); padding: 3rem; margin-bottom: 2.5rem;">
    <form id="newsletterPageForm" onsubmit="handleNewsletterSubmit(event)">
      <label style="display:block; font-size:0.65rem; letter-spacing:0.2em; text-transform:uppercase; color:var(--rose-gold); margin-bottom:0.6rem;">Your email</label>
      <div class="newsletter-input-row" style="margin-bottom:1rem;">
        <input type="email" name="email" placeholder="your@email.com" required class="newsletter-input" autocomplete="email">
        <button type="submit" class="newsletter-btn">Subscribe Free</button>
      </div>
      <p class="newsletter-fine" style="opacity:0.5; font-size:0.7rem; color:var(--cream-faint);">No spam. Unsubscribe at any time. We never sell your email address.</p>
      <div id="newsletterSuccess" style="display:none; color:var(--rose-gold-bright); font-size:0.88rem; margin-top:1rem;">✓ You're in — check your inbox for a confirmation.</div>
    </form>
  </div>

  <div style="display:grid; grid-template-columns:1fr 1fr; gap:1.25rem; margin-bottom:3rem;">
    <div style="background:rgba(255,255,255,0.02); border:0.5px solid var(--border); padding:1.5rem 1.25rem;">
      <p style="font-size:1.5rem; margin-bottom:0.5rem;">🔬</p>
      <p style="font-size:0.65rem; letter-spacing:0.2em; text-transform:uppercase; color:var(--rose-gold); margin-bottom:0.4rem;">Science Reads</p>
      <p style="font-size:0.82rem; line-height:1.7; color:var(--cream-dim);">Peer-reviewed research on sexual health, translated into something useful.</p>
    </div>
    <div style="background:rgba(255,255,255,0.02); border:0.5px solid var(--border); padding:1.5rem 1.25rem;">
      <p style="font-size:1.5rem; margin-bottom:0.5rem;">⭐</p>
      <p style="font-size:0.65rem; letter-spacing:0.2em; text-transform:uppercase; color:var(--rose-gold); margin-bottom:0.4rem;">Top Reviews</p>
      <p style="font-size:0.82rem; line-height:1.7; color:var(--cream-dim);">Our highest-scoring new products — tested over 3 weeks, scored honestly.</p>
    </div>
    <div style="background:rgba(255,255,255,0.02); border:0.5px solid var(--border); padding:1.5rem 1.25rem;">
      <p style="font-size:1.5rem; margin-bottom:0.5rem;">📖</p>
      <p style="font-size:0.65rem; letter-spacing:0.2em; text-transform:uppercase; color:var(--rose-gold); margin-bottom:0.4rem;">Buying Guides</p>
      <p style="font-size:0.82rem; line-height:1.7; color:var(--cream-dim);">Category deep-dives that tell you exactly what to buy and what to avoid.</p>
    </div>
    <div style="background:rgba(255,255,255,0.02); border:0.5px solid var(--border); padding:1.5rem 1.25rem;">
      <p style="font-size:1.5rem; margin-bottom:0.5rem;">🔒</p>
      <p style="font-size:0.65rem; letter-spacing:0.2em; text-transform:uppercase; color:var(--rose-gold); margin-bottom:0.4rem;">100% Private</p>
      <p style="font-size:0.82rem; line-height:1.7; color:var(--cream-dim);">Your subscription is private. We never share or sell subscriber data.</p>
    </div>
  </div>

  <p style="font-size:0.78rem; line-height:1.8; color:var(--cream-faint); text-align:center;">
    Sent weekly. Unsubscribe anytime via one click.<br>
    Questions? <a href="{{ '/contact/' | relative_url }}" style="color:var(--rose-gold);">Contact us</a>.
  </p>

</div>
