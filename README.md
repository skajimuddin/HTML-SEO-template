
# The Ultimate HTML SEO Template

Use this reference for creating SEO-optimized web pages. The following template covers all critical SEO, social, and technical meta tags and best practices.

---

## 1. Critical Required Tags

```html
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Your Page Title Here | Brand Name</title>
<meta name="description" content="A brief description of your page (max ~160 characters for SEO).">
```

---

## 2. Search Engine Directives

```html
<meta name="robots" content="index, follow, max-snippet:-1, max-image-preview:large, max-video-preview:-1">
<link rel="canonical" href="https://yourdomain.com/page-slug" />
```

---

## 3. Open Graph (Social Media)

```html
<meta property="og:type" content="website" />
<meta property="og:title" content="Your OG Title" />
<meta property="og:description" content="OG Description - for Facebook previews." />
<meta property="og:image" content="https://yourdomain.com/og-image.jpg" />
<meta property="og:image:width" content="1200" />
<meta property="og:image:height" content="630" />
<meta property="og:image:alt" content="Description of the image" />
<meta property="og:url" content="https://yourdomain.com/page-slug" />
<meta property="og:site_name" content="Your Site Name" />
<meta property="og:locale" content="en_US" />
```

---

## 4. Twitter Cards

```html
<meta name="twitter:card" content="summary_large_image" />
<meta name="twitter:title" content="Your Twitter Title" />
<meta name="twitter:description" content="Twitter description here" />
<meta name="twitter:image" content="https://yourdomain.com/twitter-image.jpg" />
<meta name="twitter:image:alt" content="Description of Twitter image" />
<meta name="twitter:site" content="@yourhandle" />
<meta name="twitter:creator" content="@creatorhandle" />
```

---

## 5. Favicons

```html
<link rel="icon" href="/favicon.ico" sizes="32x32" />
<link rel="icon" href="/favicon.svg" type="image/svg+xml" />
<link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png" />
<link rel="manifest" href="/site.webmanifest" />
```

---

## 6. Structured Data (Schema.org)

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "WebSite",
  "name": "Your Website Name",
  "url": "https://yourdomain.com",
  "description": "Website description",
  "potentialAction": {
    "@type": "SearchAction",
    "target": "https://yourdomain.com/search?q={search_term_string}",
    "query-input": "required name=search_term_string"
  },
  "author": {
    "@type": "Organization",
    "name": "Your Organization",
    "url": "https://yourdomain.com"
  },
  "publisher": {
    "@type": "Organization",
    "name": "Your Organization",
    "logo": {
      "@type": "ImageObject",
      "url": "https://yourdomain.com/logo.png"
    }
  }
}
</script>
```

---

## 7. Performance Optimization

```html
<link rel="dns-prefetch" href="//fonts.googleapis.com">
<link rel="dns-prefetch" href="//www.google-analytics.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="preload" href="/images/hero-image.webp" as="image">
```

---

## 8. Internationalization

```html
<link rel="alternate" hreflang="en" href="https://yourdomain.com/page-slug" />
<link rel="alternate" hreflang="x-default" href="https://yourdomain.com/page-slug" />
```

---

## 9. PWA / Mobile Meta Tags

```html
<meta name="theme-color" content="#ffffff" />
<meta name="theme-color" media="(prefers-color-scheme: dark)" content="#000000" />
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent" />
<meta name="apple-mobile-web-app-title" content="App Name" />
```

---

## 10. Security Headers

```html
<meta http-equiv="Content-Security-Policy" content="
  default-src 'self';
  script-src 'self' https://www.googletagmanager.com https://www.gstatic.com;
  style-src 'self' 'unsafe-inline' https://fonts.googleapis.com;
  font-src https://fonts.gstatic.com;
  img-src 'self' data:;
  connect-src 'self' https://firestore.googleapis.com https://identitytoolkit.googleapis.com;
">
<meta http-equiv="Referrer-Policy" content="strict-origin-when-cross-origin">
<meta http-equiv="Permissions-Policy" content="geolocation=(), microphone=(), camera=()">
```

---

## 11. Additional Structured Data (Articles, Breadcrumbs)

```html
<!-- Only for articles: -->
<meta property="article:author" content="Author Name" />
<meta property="article:published_time" content="2025-01-01T00:00:00Z" />
<meta property="article:modified_time" content="2025-01-01T00:00:00Z" />

<!-- Breadcrumb Schema (not for SPA) -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "BreadcrumbList",
  "itemListElement": [
    {
      "@type": "ListItem",
      "position": 1,
      "name": "Home",
      "item": "https://yourdomain.com"
    },
    {
      "@type": "ListItem",
      "position": 2,
      "name": "Category",
      "item": "https://yourdomain.com/category"
    }
  ]
}
</script>
```

---

## 12. Content Feeds (Blogs)

```html
<link rel="alternate" type="application/rss+xml" title="Site RSS Feed" href="/feed.xml" />
<link rel="alternate" type="application/atom+xml" title="Site Atom Feed" href="/atom.xml" />
```

---

## 13. Authorship & Metadata

```html
<meta name="author" content="Azim / Your Name or Agency">
```

---

## robots.txt 

```txt
User-agent: *
Allow: /
Disallow: /admin/

Sitemap: https://yourdomain.com/sitemap.xml
```

## llms.txt

```txt
# Your Website Name

> Brief description of what your site/business does and its main purpose.

Key information about your site or any important notes visitors should know.

## Main Content

- [About Us](https://yourdomain.com/about): Company background and mission
- [Services](https://yourdomain.com/services): What we offer and how we help
- [Blog](https://yourdomain.com/blog): Latest articles and insights

## Resources

- [Contact Info](https://yourdomain.com/contact): How to reach us
- [FAQ](https://yourdomain.com/faq): Common questions and answers

## Optional

- [Privacy Policy](https://yourdomain.com/privacy): Data handling practices
- [Terms of Service](https://yourdomain.com/terms): Usage terms
```

## sitemap.xml

```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  
  <url>
    <loc>https://yourdomain.com/</loc>
    <priority>1.0</priority>
  </url>
  
  <url>
    <loc>https://yourdomain.com/about</loc>
    <priority>0.8</priority>
  </url>
  
  <url>
    <loc>https://yourdomain.com/services</loc>
    <priority>0.8</priority>
  </url>
  
  <url>
    <loc>https://yourdomain.com/blog/post-1</loc>
    <priority>0.6</priority>
  </url>
  
</urlset>
```

## Google Analytics 4

1. Go to analytics.google.com
2. Create account → Property → Data stream
3. Copy the "Measurement ID" (starts with G-)

## Google Search Console

1. Go to search.google.com/search-console
2. Add your site as a new property (use the domain or URL prefix method).
3. Verify ownership using DNS or HTML tag method.
4. Submit your sitemap.xml file to help Google crawl your pages.

## Google Business Profile Link (for Local SEO)
1. Create or claim your profile at google.com/business.
2. Once live, copy your shareable business URL.
3. Add it to your site footer or contact page:
```html
<a href="https://g.page/your-business-id?share" target="_blank" rel="noopener">Find us on Google</a>
```


## PWA (Optional)
Helps users install your website like an app, enables offline access, faster loading, and boosts engagement.

---

<h3 align="center">
  Made by <a href="https://skajimuddin.com">Azim</a>
<h3>

---