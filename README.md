# Google Analytics integration: Track user behavior and website performance

Understanding your website's performance is crucial for growth, and Google Analytics is your secret weapon. Integrating it into your Webflow site unlocks a treasure trove of insights, but the code can seem daunting. Fear not, brave developer, for we'll navigate this together with a clean code example!

**1. Webflow's Analytics Superpower:**

  - **Track website traffic:** Understand how users navigate your site, identify popular pages, and analyze conversion funnels.
  - **Measure visitor engagement:** Gauge time spent on pages, bounce rates, and scroll depth for deeper user understanding.
  - **Gain valuable insights:** Drive data-driven decisions based on user behavior, optimize your content, and improve your website's effectiveness.

**2. Integration Options:**

  - **Webflow built-in:** No coding required, simply enter your Google Analytics tracking ID in the site settings.
  - **GTM (Google Tag Manager):** Offers fine-grained control and advanced tracking capabilities for complex websites.
  - **Custom code injection:** For ultimate flexibility and unique tracking needs.

**3. Short & Clean Code Example (GTM):**

```
HTML
<script src="https://www.googletagmanager.com/gtm.js?id=GTM-YOUR_ID"></script>
<noscript><iframe src="https://www.googletagmanager.com/ns.html?id=GTM-YOUR_ID" height="0" width="0" style="display:none;visibility:hidden"></iframe></noscript>

<script>
  window.addEventListener('WebflowPageReady', function() {
    dataLayer.push({
      event: 'pageview'
    });
  });
</script>

<script>
  // Track form submissions
  document.getElementById('contact-form').addEventListener('submit', function() {
    dataLayer.push({
      event: 'contact_form_submit'
    });
  });
</script>
```
# Need Help?
Need custom [Webflow Development](https://epyc.in/)?
