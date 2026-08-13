# Hamis Gaming Empire - Project Structure & Documentation

## 📋 Project Overview

**Repository**: hamis-gaming-empire (GitHub: mwaka991)  
**Website**: RisTechy.com - A gaming & technology blog  
**Type**: Static Website Mirror (HTTrack Website Copy)  
**Size**: 119MB | 565 HTML files | 364,338+ lines of code  
**Status**: Locally hosted mirror with 448 directories

---

## 🎯 Project Purpose

This is a complete offline mirror of **ristechy.com**, a technology blog featuring:
- Android game downloads & mods (APK files)
- Game reviews and tutorials
- Software guides and tips

The site was captured/mirrored using **HTTrack Website Copier v3.49-6** for offline browsing.

---

## 📁 Directory Structure

```
hamis-gaming-empire/
├── index.html                    # Root landing page (HTTrack mirror index)
├── README.md                     # Project readme
├── hts-log.txt                   # HTTrack mirror log
├── hts-cache/                    # HTTrack cache files
│   ├── new.lst                   # List of new/updated files
│   └── new.txt                   # New files text log
├── backblue.gif                  # Background image asset
├── fade.gif                       # Fade effect asset
├── .git/                         # Git repository metadata
└── ristechy.com/                 # Main website mirror (119MB, 448 subdirs)
    ├── index.html                # Homepage
    ├── about.html                # About page
    ├── contact.html              # Contact form page
    ├── android.html              # Android section
    ├── 404.html                  # Error page
    │
    ├── [Game/App Pages] - 565 total HTML files:
    │   ├── 8-ball-pool-apk-mod.html
    │   ├── dream-league-soccer-2024-dls-24-mod-apk.html
    │   ├── fifa-2025-mod-fifa-14-fc-apk-offline.html
    │   ├── asphalt-9-legends-apk-mod-android.html
    │   ├── gta-san-andreas-apk-obb-highly-compressed.html
    │   └── [... and 560+ more game/app pages]
    │
    ├── [Directories matching game pages] - 448 subdirs:
    │   ├── 8-ball-pool-apk-mod/
    │   ├── dream-league-soccer-2024-dls-24-mod-apk/
    │   └── [... subdirectories for related assets/pages]
    │
    └── wp-content/               # WordPress theme/plugin assets
        ├── cache/                # Cached minified CSS/JS
        ├── plugins/              # Installed plugins (WM Video Playlists, Shortcodes Ultimate)
        ├── themes/               # Theme files (Jannah theme v7.6.5)
        ├── uploads/              # Media uploads (images, featured images)
        └── [... other WP assets]
```

---

## 🔗 Page Communication & Navigation

### **Navigation Architecture**

The website uses a **common WordPress theme (Jannah)** with consistent navigation:

1. **Global Navigation Bar**
   - Main menu with category links
   - Logo/branding
   - Search functionality
   - Social media links

2. **Main Categories** (linked throughout site):
   - Home (`index.html` / `ristechy.com/`)
   - About (`about.html`)
   - Contact (`contact.html`)
   - Android section (`android.html`)
   - Game/App categories (e.g., "Android Games", "Sports Betting Apps")

3. **Cross-page Communication Methods**:

   **a) Relative Links**
   - All internal links use relative paths (e.g., `href="about.html"`)
   - Example: Game pages link to `contact.html` for support
   - Archive pages link to category pages

   **b) Breadcrumb Navigation**
   - Schema markup includes breadcrumb trails
   - Example: Home > Android Games > [Game Name]
   - Helps users understand site hierarchy

   **c) Related Links**
   - Game pages link to related games in same category
   - Example: DLS 2024 links to DLS 2023, DLS 2022, etc.
   - Footer navigation provides quick access to main sections

   **d) Meta & Schema**
   - JSON-LD schema tags define page relationships
   - OG meta tags for social sharing
   - Canonical tags prevent duplicate content issues

### **Page Structure Pattern** (Consistent across all 565 pages)

Each HTML page follows this structure:

```html
<!DOCTYPE html>
<html lang="en-US">
<head>
  <!-- Meta Tags (SEO, OG, Schema JSON-LD) -->
  <meta charset="UTF-8">
  <title>[Page Title] - RisTechy.com</title>
  
  <!-- Stylesheets -->
  <link rel='stylesheet' href='wp-content/themes/jannah/assets/css/base.min.css'>
  <link rel='stylesheet' href='wp-content/themes/jannah/assets/css/style.min.css'>
  
  <!-- Scripts (lazy loaded) -->
  <script type="text/rocketlazyloadscript" id="jquery-core-js" 
    data-rocket-src="wp-includes/js/jquery/jquery.min.js"></script>
</head>

<body id="tie-body" class="[page-specific-classes]">
  <div id="tie-container" class="site">
    <!-- Navigation Header -->
    <div id="tie-wrapper">
      <header id="tie-header">
        <!-- Logo, Main Nav, Search Bar -->
      </header>
      
      <!-- Main Content -->
      <main id="the-post">
        <article>
          <h1>[Page Title]</h1>
          <div class="entry-content">
            <!-- Article/Page Content -->
          </div>
        </article>
        
        <!-- Related Posts/Links Section -->
        <div class="related-posts">
          <!-- Links to similar pages -->
        </div>
      </main>
      
      <!-- Sidebar (optional) -->
      <aside id="sidebar">
        <!-- Widgets, Related Content -->
      </aside>
      
      <!-- Footer -->
      <footer id="tie-footer">
        <!-- Footer Menu, Copyright, Social Links -->
      </footer>
    </div>
  </div>
</body>
</html>
```

---

## 🎨 Technology Stack

### **Frontend**
- **HTML5**: Standard markup
- **CSS**: Multiple stylesheets (base, style, widgets, single, print, helpers)
- **JavaScript**: jQuery 3.7.1 + lazy loading
- **Rocket Lazy Load**: Performance optimization for scripts/images
- **Font**: Questrial (Google Fonts)

### **WordPress Theme**
- **Theme**: Jannah v7.6.5 (Magazine/news theme)
- **Theme Features**:
  - Responsive design (mobile-first)
  - Dark mode support (`data-skin="light"`)
  - Magazine-style layouts
  - SEO optimized (Yoast SEO Premium v28.2)
  - Performance optimized (Rocket optimization)

### **Plugins Used**
- **WM Video Playlists**: Embedded video management
- **Shortcodes Ultimate**: Enhanced content formatting
- **Yoast SEO Premium**: SEO optimization
- **Rocket** (WP Rocket): Caching & performance



---

## 📊 File Statistics

| Metric | Value |
|--------|-------|
| Total HTML Files | 418 |
| Total Directories | 400+ |
| Total Lines of Code | 285,000+ |
| Project Size | 95 MB |
| Game Pages | 410+ |
| Index Variations | Multiple (index000a.html, index00ae.html, etc.) |
| Main Pages | ~5 (index, about, contact, android, 404) |

---

## 🚀 How Pages Are Organized

### **By Category**
1. **Games** (majority - 400+ pages)
   - Android Games (Dream League, FIFA, Asphalt, etc.)
   - Emulated Games (PPSSPP, DamonPS2, etc.)
   - Strategy/Casual Games (Dragon City, Clash Royale, etc.)

2. **Static Pages** (5 pages)
   - Landing page (index.html)
   - About (about.html)
   - Contact (contact.html)
   - Android section (android.html)
   - Error page (404.html)

### **Naming Convention**
- Slugified page names: `game-name-apk-mod.html`
- Example: `dream-league-soccer-2024-dls-24-mod-apk.html`
- Matching subdirectories for assets: `dream-league-soccer-2024-dls-24-mod-apk/`

---

## 🔄 Page Communication Flow

```
Root Index (index.html)
    ↓
    ├→ Redirects to ristechy.com/index.html
    └→ Contains HTTrack mirror index listing

Main Navigation (on all pages)
    ├→ About Page
    ├→ Contact Page
    ├→ Android Section
    ├→ Category Archives
    └→ Search

Game/App Pages (550+ pages)
    ├→ Link to Related games in same category
    ├→ Link to Contact for support
    ├→ Link to About for information
    └→ Social sharing (OG meta tags)

Footer (all pages)
    ├→ Main navigation links
    ├→ Social media links
    ├→ Copyright info
    └→ RSS feeds
```

---

## 📝 Key Files to Understand

| File | Purpose |
|------|---------|
| `/index.html` | HTTrack mirror landing page |
| `/ristechy.com/index.html` | Main website homepage |
| `/ristechy.com/about.html` | About RisTechy info |
| `/ristechy.com/contact.html` | Contact form (static) |
| `hts-log.txt` | Mirror operation log |
| `wp-content/themes/jannah/` | Theme templates & styles |
| `wp-content/plugins/` | Plugin functionality |
| `wp-content/uploads/` | Media assets (images) |

---

## 🌐 How to Access the Site

### **Local Development**
1. Run HTTP server: `python3 -m http.server 8000`
2. Access: `http://localhost:8000/ristechy.com/`
3. Or through Codespace: Port forward and access via browser

### **Live Mirror**
- Original: https://ristechy.com
- Mirror Status: Offline copy (as of Aug 2026)

---

## 💡 Important Notes

1. **Static Mirror**: All dynamic features (comments, forms) won't work locally
2. **External Dependencies**: Some images/scripts may reference external CDNs
3. **Responsive Design**: Pages are mobile-responsive
4. **SEO Optimized**: Includes structured data (JSON-LD) and meta tags
5. **Large Project**: 119MB size, best served locally with HTTP server

---

## 📚 Navigation Summary

**How pages communicate**:
- ✅ Relative links (within site structure)
- ✅ Breadcrumb navigation (via schema markup)
- ✅ Category/related links
- ✅ Footer navigation
- ✅ Social meta tags (OG tags)
- ✅ Search functionality
- ❌ Dynamic features (forms don't submit locally)
- ❌ Analytics & advertising (removed)

---

*Last Updated: August 13, 2026*  
*Mirror Created: August 10, 2026 (HTTrack v3.49-6)*  
*Cleanup: August 13, 2026 (Removed VPN, Sports Betting, Utility apps, Communication page, Analytics & Ads)*
