<template>
  <div class="wedding-page">

    <!-- Hero Section -->
    <section class="hero" :style="{ backgroundImage: 'url(/image/weeding_01.jpg)' }">
      <div class="hero-overlay">
        <p class="hero-sub">သဘောတူညီမှုနှင့် ချစ်ခြင်းမေတ္တာဖြင့်</p>
        <h1 class="hero-title">ဒေါက်တာသက်ဇင်ထူး</h1>
        <div class="hero-divider">
          <span class="divider-line"></span>
          <span class="divider-heart">♡</span>
          <span class="divider-line"></span>
        </div>
        <h1 class="hero-title">မခန့်ကေသွယ်</h1>
        <p class="hero-date">၂၀၂၆ ခုနှစ် မေလ ၂၃ ရက်</p>
        <a href="#invitation" class="hero-btn">ဖိတ်ကြားလွှာ ကြည့်ရှုရန်</a>
      </div>
    </section>

    <!-- Invitation Letter Section -->
    <section id="invitation" class="invitation-section">
      <div class="section-header">
        <p class="section-label">Wedding Invitation</p>
        <h2 class="section-title">မင်္ဂလာပွဲ ဖိတ်ကြားလွှာ</h2>
        <div class="title-ornament">✦ ✦ ✦</div>
      </div>
      <div class="invitation-card">
        <img
          src="/image/invitationg_letter.jpg"
          alt="မင်္ဂလာပွဲ ဖိတ်ကြားလွှာ"
          class="invitation-img"
        />
      </div>
    </section>

    <!-- Event Details Section -->
    <section class="event-section">
      <div class="section-header">
        <p class="section-label">Wedding Ceremony</p>
        <h2 class="section-title">စုလျားရစ်ပတ်ထိမ်းမြားမင်္ဂလာအစီအစဉ်</h2>
        <div class="title-ornament">✦ ✦ ✦</div>
      </div>
      <div class="event-card">
        <div class="event-item">
          <div class="event-icon">❤️</div>
          <h3 class="event-label">မင်္ဂလာနေ့ရက်</h3>
          <p class="event-value">၁၃၈၈-ခုနှစ်၊ နယုန်လဆန်း(၈)ရက်</p>
          <p class="event-value">23.5.2026 (စနေနေ့)</p>
        </div>
        <div class="event-divider"></div>
        <div class="event-item">
          <div class="event-icon">❤️</div>
          <h3 class="event-label">မင်္ဂလာအချိန်</h3>
          <p class="event-value">နံနက် (၈:၀၀) နာရီမှ (၁၁:၀၀) နာရီအထိ</p>
        </div>
        <div class="event-divider"></div>
        <div class="event-item">
          <div class="event-icon">❤️</div>
          <h3 class="event-label">မင်္ဂလာနေရာ</h3>
          <p class="event-value">"မဏိကဉ္စနာ ခန်းမ"</p>
          <p class="event-value">မြင်းခြံမြို့</p>
        </div>
      </div>
    </section>

    <!-- QR Section -->
    <section class="qr-section">
      <div class="section-header">
        <p class="section-label">Gift & Blessing</p>
        <h2 class="section-title">လက်ဆောင် ပေးပို့ရန်</h2>
        <div class="title-ornament">✦ ✦ ✦</div>
      </div>
      <div class="qr-card">
        <p class="qr-desc">KBZ Pay မှတဆင့် ကြင်နာသောလက်ဆောင် ပေးပို့နိုင်ပါသည်</p>
        <div class="qr-wrapper">
          <img
            src="/image/kbz-qr.jpg"
            alt="KBZ Pay QR Code"
            class="qr-img"
          />
        </div>
        <p class="qr-note">QR Code ကို Scan ပြုလုပ်ပေးပါ</p>
      </div>
    </section>

    <!-- Footer -->
    <footer class="wedding-footer">
      <p class="footer-names">ဒေါက်တာသက်ဇင်ထူး ♡ မခန့်ကေသွယ်</p>
      <p class="footer-wish">ကျွန်ုပ်တို့၏ မင်္ဂလာပွဲသို့ ကြွရောက်ပေးသည့်အတွက် အထူးကျေးဇူးတင်ပါသည်</p>
    </footer>

  </div>
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Segoe UI', 'Pyidaungsu', sans-serif;
  background: #fdf8f3;
  color: #3d2b1f;
}

/* ── Hero ── */
.hero {
  min-height: 100svh;
  background-size: cover;
  background-position: center top;
  background-repeat: no-repeat;
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
}

.hero-overlay {
  background: linear-gradient(to bottom, rgba(0,0,0,0.35) 0%, rgba(0,0,0,0.55) 100%);
  position: absolute;
  inset: 0;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 2rem;
  text-align: center;
  gap: 0.75rem;
}

.hero-sub {
  color: #f5deb3;
  font-size: 0.95rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
}

.hero-title {
  font-size: clamp(2.2rem, 8vw, 4.5rem);
  color: #fff;
  font-weight: 300;
  letter-spacing: 0.06em;
  text-shadow: 0 2px 12px rgba(0,0,0,0.4);
  font-style: italic;
}

.hero-divider {
  display: flex;
  align-items: center;
  gap: 0.75rem;
  width: 100%;
  max-width: 280px;
  margin: 0.25rem 0;
}

.divider-line {
  flex: 1;
  height: 1px;
  background: rgba(245, 222, 179, 0.7);
}

.divider-heart {
  color: #f5c6c6;
  font-size: 1.4rem;
}

.hero-date {
  color: #f5deb3;
  font-size: 1rem;
  letter-spacing: 0.1em;
  margin-top: 0.5rem;
}

.hero-btn {
  display: inline-block;
  margin-top: 1.5rem;
  padding: 0.7rem 2rem;
  border: 1.5px solid rgba(245, 222, 179, 0.8);
  color: #f5deb3;
  text-decoration: none;
  font-size: 0.9rem;
  letter-spacing: 0.1em;
  border-radius: 50px;
  transition: background 0.3s, color 0.3s;
}

.hero-btn:hover {
  background: rgba(245, 222, 179, 0.2);
}

/* ── Shared Section Styles ── */
.section-header {
  text-align: center;
  margin-bottom: 2rem;
}

.section-label {
  font-size: 0.8rem;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  color: #b5845a;
  margin-bottom: 0.5rem;
}

.section-title {
  font-size: clamp(1.5rem, 5vw, 2.2rem);
  font-weight: 400;
  color: #3d2b1f;
  letter-spacing: 0.04em;
}

.title-ornament {
  color: #c9a87c;
  font-size: 0.75rem;
  letter-spacing: 0.5em;
  margin-top: 0.75rem;
}

/* ── Invitation Section ── */
.invitation-section {
  padding: 4rem 1.25rem;
  background: #fdf8f3;
}

.invitation-card {
  max-width: 560px;
  margin: 0 auto;
  border-radius: 16px;
  overflow: hidden;
  box-shadow: 0 8px 40px rgba(0,0,0,0.12);
}

.invitation-img {
  width: 100%;
  height: auto;
  display: block;
}

/* ── Event Details Section ── */
.event-section {
  padding: 4rem 1.25rem;
  background: #fdf8f3;
}

.event-card {
  max-width: 560px;
  margin: 0 auto;
  background: #fff;
  border-radius: 20px;
  padding: 2.5rem 2rem;
  box-shadow: 0 8px 40px rgba(0,0,0,0.1);
  border: 1px solid #f5e6d3;
}

.event-item {
  text-align: center;
  padding: 1.25rem 0;
}

.event-icon {
  font-size: 1.4rem;
  margin-bottom: 0.5rem;
}

.event-label {
  font-size: 1rem;
  font-weight: 600;
  color: #b5845a;
  letter-spacing: 0.06em;
  margin-bottom: 0.5rem;
}

.event-value {
  font-size: 1rem;
  color: #3d2b1f;
  line-height: 1.8;
}

.event-divider {
  height: 1px;
  background: linear-gradient(to right, transparent, #f5deb3, transparent);
  margin: 0.25rem 0;
}

/* ── QR Section ── */
.qr-section {
  padding: 4rem 1.25rem;
  background: linear-gradient(135deg, #fff8f0 0%, #fdeee0 100%);
}

.qr-card {
  max-width: 360px;
  margin: 0 auto;
  text-align: center;
  background: #fff;
  border-radius: 20px;
  padding: 2rem 1.5rem;
  box-shadow: 0 8px 40px rgba(0,0,0,0.1);
}

.qr-desc {
  font-size: 0.9rem;
  color: #7a5c44;
  line-height: 1.7;
  margin-bottom: 1.5rem;
}

.qr-wrapper {
  border-radius: 12px;
  overflow: hidden;
  border: 3px solid #f5deb3;
}

.qr-img {
  width: 100%;
  height: auto;
  display: block;
}

.qr-note {
  margin-top: 1.25rem;
  font-size: 0.85rem;
  color: #b5845a;
  letter-spacing: 0.05em;
}

/* ── Footer ── */
.wedding-footer {
  background: #3d2b1f;
  color: #f5deb3;
  text-align: center;
  padding: 2.5rem 1.25rem;
}

.footer-names {
  font-size: 1.25rem;
  letter-spacing: 0.08em;
  font-style: italic;
  margin-bottom: 0.75rem;
}

.footer-wish {
  font-size: 0.85rem;
  color: rgba(245, 222, 179, 0.7);
  line-height: 1.8;
}

/* ── Mobile tweaks ── */
@media (max-width: 480px) {
  .hero-btn {
    padding: 0.6rem 1.5rem;
    font-size: 0.85rem;
  }

  .qr-card {
    padding: 1.5rem 1rem;
  }
}
</style>
