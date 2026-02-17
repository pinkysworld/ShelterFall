# Shelter Fall — Website

Official website for **Shelter Fall**, a post-apocalyptic survival strategy game for iOS.

## 🌐 Pages

| Page | File | Description |
|------|------|-------------|
| Landing Page | `index.html` | Marketing page with features, gameplay, and App Store link |
| Privacy Policy | `privacy.html` | Required for App Store — covers AdMob, ATT, data practices |
| Terms of Service | `terms.html` | Usage terms for the app |
| Support | `support.html` | FAQ and contact information |
| Press Kit | `presskit.html` | Media resources and game facts |

## 🚀 Deploy to GitHub Pages

### Option 1 — Dedicated Repository (Recommended)

1. Create a new GitHub repository named `shelter-fall`
2. Copy the contents of this `website/` folder into the repo root:
   ```bash
   cd website
   git init
   git add .
   git commit -m "Initial website"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/shelter-fall.git
   git push -u origin main
   ```
3. Go to **Settings → Pages** in the repository
4. Under **Source**, select **Deploy from a branch**
5. Choose **main** branch, **/ (root)** folder
6. Click **Save**
7. Your site will be live at: `https://YOUR_USERNAME.github.io/shelter-fall/`

### Option 2 — Subdirectory of Existing Repo

Copy the `website/` folder contents into a `docs/` folder of your existing repo, then set GitHub Pages source to the `docs/` folder.

## 📝 Customization Checklist

Before deploying, update these placeholders:

- [ ] Replace `YOUR_GITHUB_USERNAME` in all HTML files with your actual GitHub username
- [ ] Replace `YOUR_APP_ID` in App Store links with your actual App Store app ID
- [ ] Replace `support@shelterfall.com` with your actual support email
- [ ] Add your app icon images to the `images/` folder (see below)
- [ ] Add App Store screenshots to `images/` if desired

## 🖼️ Required Images

Place these files in the `images/` folder:

| File | Size | Usage |
|------|------|-------|
| `app-icon-1024.png` | 1024×1024 | Press kit download |
| `app-icon-512.png` | 512×512 | Hero section, navigation, Open Graph |
| `app-icon-180.png` | 180×180 | Apple touch icon |
| `app-icon-32.png` | 32×32 | Favicon |

You can generate these from the 1024px icon in the `AppIcons/` folder:

```bash
# From the ShelterFall project root
cp AppIcons/AppIcons/concept3_shelter.png website/images/app-icon-1024.png
sips -z 512 512 website/images/app-icon-1024.png --out website/images/app-icon-512.png
sips -z 180 180 website/images/app-icon-1024.png --out website/images/app-icon-180.png
sips -z 32 32 website/images/app-icon-1024.png --out website/images/app-icon-32.png
```

## 📋 App Store Connect URLs

Once deployed, use these URLs in App Store Connect:

| Field | URL |
|-------|-----|
| **Support URL** | `https://YOUR_USERNAME.github.io/shelter-fall/support.html` |
| **Marketing URL** | `https://YOUR_USERNAME.github.io/shelter-fall/` |
| **Privacy Policy URL** | `https://YOUR_USERNAME.github.io/shelter-fall/privacy.html` |

## License

© 2025 Shelter Fall. All rights reserved.
