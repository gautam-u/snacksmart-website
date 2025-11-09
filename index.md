---
layout: default
title: SnackSmart - AI-Powered Nutrition Tracking for iOS
---

<div class="hero animate-fade-in-up">
  <h1 class="text-gradient">SnackSmart<br>AI-Powered Nutrition</h1>
  <p class="mb-xl">SnackSmart brings intelligent nutrition tracking to your iPhone with instant AI food recognition, personalized insights, and seamless HealthKit sync. Start free with unlimited scans, then upgrade to Premium for advanced analytics and ad-free experience — all while your data stays securely on your device.</p>
  <p class="mb-2xl" style="color: var(--color-text-secondary); max-width: 680px; margin-left: auto; margin-right: auto;">Monthly and yearly Premium memberships unlock advanced nutrition analytics, custom dietary filters, and priority AI processing for serious health enthusiasts.</p>

  <div style="display: flex; justify-content: center; margin-bottom: var(--spacing-4xl);">
    <a href="{{ site.appstore_link | default: '#' }}" class="btn btn-primary btn-large">
      <i class="fab fa-apple"></i>
      Get SnackSmart on the App Store
    </a>
  </div>
</div>

<div class="screenshots">
  <div class="screenshot">
    <img src="{{ '/assets/screenshots/dashboard.png' | relative_url }}" alt="SnackSmart Dashboard with AI Insights">
  </div>
  <div class="screenshot">
    <img src="{{ '/assets/screenshots/camera.png' | relative_url }}" alt="AI-powered food recognition camera">
  </div>
  <div class="screenshot">
    <img src="{{ '/assets/screenshots/healthkit.png' | relative_url }}" alt="HealthKit integration and sync">
  </div>
  <div class="screenshot">
    <img src="{{ '/assets/screenshots/premium.png' | relative_url }}" alt="Premium membership benefits">
  </div>
  <div class="screenshot">
    <img src="{{ '/assets/screenshots/analytics.png' | relative_url }}" alt="Advanced nutrition analytics dashboard">
  </div>
  <div class="screenshot">
    <img src="{{ '/assets/screenshots/history.png' | relative_url }}" alt="Unlimited snack history tracking">
  </div>
</div>

<section class="features">
  <div class="text-center mb-2xl">
    <h2>Smarter Snacking with AI</h2>
    <p>On-device intelligence, instant recognition, and seamless HealthKit sync for complete nutrition tracking.</p>
  </div>

  <div class="grid grid-3">
    {% for feature in site.features %}
    <div class="card feature-card animate-fade-in-up">
      <div class="feature-icon">
        <i class="fas fa-{{ feature.fontawesome_icon_name }}"></i>
      </div>
      <h3>{{ feature.title }}</h3>
      <p>{{ feature.description }}</p>
    </div>
    {% endfor %}
  </div>
</section>

<section class="features">
  <div class="text-center mb-2xl">
    <h2>Flexible Premium Memberships</h2>
    <p>Choose the upgrade path that matches your wellness goals and unlock the full premium experience.</p>
  </div>

  <div class="grid grid-2">
    <div class="card feature-card animate-fade-in-up">
      <div class="feature-icon">
        <i class="fas fa-calendar-check"></i>
      </div>
      <h3>Monthly Premium Access</h3>
      <p>Stay flexible with a monthly membership that delivers ad-free tracking, advanced analytics, and unlimited exports. Perfect for trying Premium.</p>
      <p style="font-size: 1.5rem; font-weight: 700; color: var(--color-primary-blue); margin-top: var(--spacing-lg);">$2.99/month</p>
    </div>
    <div class="card feature-card animate-fade-in-up">
      <div class="feature-icon">
        <i class="fas fa-award"></i>
      </div>
      <h3>Yearly Premium Access</h3>
      <p>Save 44% with our best-value plan, including exclusive insights, deeper analytics, and priority AI processing for serious nutrition tracking.</p>
      <p style="font-size: 1.5rem; font-weight: 700; color: var(--color-primary-green); margin-top: var(--spacing-lg);">$19.99/year <span style="font-size: 0.9rem; color: var(--color-text-secondary);">(Save 44%)</span></p>
    </div>
  </div>
</section>

<section class="features" style="background: linear-gradient(135deg, var(--color-primary-blue), var(--color-primary-green)); color: white; padding: var(--spacing-4xl) var(--spacing-xl); border-radius: var(--radius-xl); margin-top: var(--spacing-4xl);">
  <div class="text-center">
    <h2 style="color: white;">Free Tier Benefits</h2>
    <p style="color: rgba(255, 255, 255, 0.9); font-size: 1.1rem; max-width: 600px; margin: 0 auto;">SnackSmart is completely free to use with unlimited scans. Occasional ads every 7 scans help support development. Upgrade anytime for ad-free experience and premium features.</p>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: var(--spacing-xl); margin-top: var(--spacing-2xl);">
      <div style="text-align: center;">
        <i class="fas fa-infinity" style="font-size: 2.5rem; margin-bottom: var(--spacing-md);"></i>
        <h4 style="color: white; margin-bottom: var(--spacing-sm);">Unlimited Scans</h4>
        <p style="color: rgba(255, 255, 255, 0.8); font-size: 0.9rem; margin: 0;">Track every snack, no daily limits</p>
      </div>
      <div style="text-align: center;">
        <i class="fas fa-brain" style="font-size: 2.5rem; margin-bottom: var(--spacing-md);"></i>
        <h4 style="color: white; margin-bottom: var(--spacing-sm);">AI Recognition</h4>
        <p style="color: rgba(255, 255, 255, 0.8); font-size: 0.9rem; margin: 0;">Full AI-powered food detection</p>
      </div>
      <div style="text-align: center;">
        <i class="fas fa-heartbeat" style="font-size: 2.5rem; margin-bottom: var(--spacing-md);"></i>
        <h4 style="color: white; margin-bottom: var(--spacing-sm);">HealthKit Sync</h4>
        <p style="color: rgba(255, 255, 255, 0.8); font-size: 0.9rem; margin: 0;">Seamless Apple Health integration</p>
      </div>
    </div>
  </div>
</section>
