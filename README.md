# 🎨 HaKai Art Agency - Deployment & Setup Guide

Welcome **Trần Đình Tuấn**! This repository contains the complete source code for **HaKai Art Agency** digital art showcase. Below is a simple step-by-step guide to hosting your site for free on **GitHub Pages** with your custom domain.

---

## 📁 1. Project Directory Structure

```
hakai-art-agency/
├── index.html              # Main website layout (English)
├── CNAME                   # Custom domain configuration file
├── README.md               # Documentation guide
├── css/
│   ├── style.css           # Core design system & typography (Be Vietnam Pro & Montserrat)
│   └── components.css      # Component styling (Gallery, Modals, Uploader)
├── js/
│   ├── app.js              # Application logic, deep linking & hash routing
│   ├── storage.js          # IndexedDB browser storage manager
│   └── data.js             # Initial template artworks
└── assets/
    └── images/             # Sample high-res artworks (artwork_1.jpg, ...)
```

---

## 🚀 2. Deploying to GitHub Pages

### **Step 1: Create a Repository**
1. Sign in to [GitHub.com](https://github.com).
2. Click **`+`** (top right) -> Select **New repository**.
3. Name your repository (e.g., `hakai-art-agency` or `hakai-portfolio`).
4. Set visibility to **Public**.
5. Click **Create repository**.

### **Step 2: Upload Files**
1. On the repository setup page, click **"uploading an existing file"**.
2. Drag and drop all files and folders inside `hakai-art-agency` into GitHub.
3. Scroll down and click **Commit changes**.

### **Step 3: Enable GitHub Pages**
1. Navigate to **Settings** -> **Pages** (left navigation bar).
2. Under **Build and deployment** -> **Branch**:
   - Select **`main`** (or `master`).
   - Leave folder as **`/ (root)`**.
   - Click **Save**.
3. After 1 - 2 minutes, refresh the page. Your site URL will be live at `https://your-username.github.io/hakai-art-agency/`.

---

## 🌐 3. Connecting Your Custom Domain

1. Edit the `CNAME` file in your repository and set it to your custom domain name (e.g. `yourdomain.com`).
2. Log into your domain registrar (e.g., Cloudflare, GoDaddy, Namecheap, Mắt Bão) and set up the following DNS records:

**A Records (for root domain):**
- **Type**: `A` | **Host**: `@` | **Value**: `185.199.108.153`
- **Type**: `A` | **Host**: `@` | **Value**: `185.199.109.153`
- **Type**: `A` | **Host**: `@` | **Value**: `185.199.110.153`
- **Type**: `A` | **Host**: `@` | **Value**: `185.199.111.153`

**CNAME Record (for www subdomain):**
- **Type**: `CNAME` | **Host**: `www` | **Value**: `your-username.github.io`

---

## 🌟 4. Features Included

- 🎨 **Luxury Dark Aesthetics**: Built with Cyber Obsidian (`#07090e`), Neon Gold (`#ffc83b`), and sleek glassmorphism.
- 📤 **Media Uploader**: Drag & drop support for high-res images and videos.
- 💾 **IndexedDB Persistence**: Uploaded media automatically persists in browser local storage.
- 🔗 **Direct Artwork Links**: Every artwork generates its own unique shareable URL hash (`#artwork-...`).
- 🔍 **Search & Filter**: Filter by Visual Art, Digital Art, 3D Art, and Video & Animation.

---
*Created for **Trần Đình Tuấn** & **HaKai Art Agency**.*
