# The Ultimate HTML SEO Template

Use this reference for creating SEO-optimized HTML pages.


## 🔹 Title & Basic SEO

```html
<title>Your Page Title Here | Brand Name</title>
<meta name="description" content="A brief description of your page (max ~160 characters for SEO).">
<meta name="author" content="Azim / Your Name or Agency">
```

---

## 🔹 Robots & Crawling

```html
<meta name="robots" content="index, follow, max-snippet:-1, max-image-preview:large, max-video-preview:-1">
<meta name="googlebot" content="index, follow">
<meta name="bingbot" content="index, follow">
```

---

## 🔹 Language & Location

```html
<meta name="language" content="English">
<meta name="geo.region" content="US">
<meta name="geo.placename" content="City, State">
```

---

## 🔹 Canonical & Alternate URLs

```html
<link rel="canonical" href="https://yourdomain.com/page-slug" />
<link rel="alternate" hreflang="en" href="https://yourdomain.com/page-slug" />
<link rel="alternate" hreflang="x-default" href="https://yourdomain.com/page-slug" />
```

---

## 🔹 Performance Tags (Prefetch, Preconnect, Preload)

```html
<link rel="dns-prefetch" href="//fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="preload" href="/css/critical.css" as="style">
<link rel="preload" href="/fonts/main-font.woff2" as="font" type="font/woff2" crossorigin="anonymous">
```

---

## 🔹 Open Graph (Facebook, LinkedIn, etc.)

```html
<meta property="og:type" content="website" />
<meta property="og:title" content="Your OG Title" />
<meta property="og:description" content="OG Description - for Facebook previews." />
<meta property="og:image" content="https://yourdomain.com/og-image.jpg" />
<meta property="og:url" content="https://yourdomain.com/page-slug" />
<meta property="og:site_name" content="Your Site Name" />
```

---

## 🔹 Twitter Cards

```html
<meta name="twitter:card" content="summary_large_image" />
<meta name="twitter:title" content="Your Twitter Title" />
<meta name="twitter:description" content="Twitter description here" />
<meta name="twitter:image" content="https://yourdomain.com/twitter-image.jpg" />
```

---

## 🔹 Favicons

```html
<link rel="icon" href="/favicon.ico" sizes="32x32" />
<link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png" />
<link rel="manifest" href="/site.webmanifest" />
```

---

## 🔹 PWA / Mobile Meta Tags

```html
<meta name="theme-color" content="#ffffff" />
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent" />
```

---

## 🔹 Security Headers

```html
<meta http-equiv="Content-Security-Policy" content="default-src 'self';">
<meta http-equiv="Referrer-Policy" content="strict-origin-when-cross-origin">
<meta http-equiv="Permissions-Policy" content="geolocation=(), microphone=(), camera=()">
```

---

## 🔹 Structured Data / Schema.org (WebSite + WebPage)

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "WebSite",
  "name": "Your Website Name",
  "url": "https://yourdomain.com"
}
</script>

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "WebPage",
  "name": "Page Title",
  "url": "https://yourdomain.com/page-slug",
  "description": "Page description"
}
</script>
```

---

## 🔹 Optional: FAQ Schema

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [{
    "@type": "Question",
    "name": "What is SEO?",
    "acceptedAnswer": {
      "@type": "Answer",
      "text": "SEO is the process of improving a site's visibility in search engines."
    }
  }]
}
</script>
```

---

## 🔹 Site Verification

```html
<meta name="google-site-verification" content="your-verification-code" />
<meta name="msvalidate.01" content="bing-verification-code" />
```

---

## 🔹 RSS / Feeds

```html
<link rel="alternate" type="application/rss+xml" title="Site RSS Feed" href="/feed.xml" />
<link rel="alternate" type="application/atom+xml" title="Site Atom Feed" href="/atom.xml" />
```

---

## 🔹 Analytics (Google, Clarity)

```html
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>

<script type="text/javascript">
  (function(c,l,a,r,i,t,y){
      c[a]=c[a]||function(){(c[a].q=c[a].q||[]).push(arguments)};
      t=l.createElement(r);t.async=1;t.src="https://www.clarity.ms/tag/"+i;
      y=l.getElementsByTagName(r)[0];y.parentNode.insertBefore(t,y);
  })(window, document, "clarity", "script", "YOUR_CLARITY_ID");
</script>
```

---

✅ **Use this Markdown to copy and paste into your projects.**

Use Google’s Rich Results Test to see if it’s valid:
👉 https://search.google.com/test/rich-results