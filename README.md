# 🎂 Happy Birthday Noshi - Interactive Birthday Card

A beautiful, animated birthday card website with music, interactive elements, and a downloadable PDF card.

## ✨ Features

- 🎵 **Auto-play Background Music** - Plays "UDI UDI.mp3" automatically after login
- 🔐 **Password Protection** - Login page with security question
- 📱 **Fully Responsive** - Works perfectly on desktop, tablet, and mobile devices
- 🎨 **Beautiful Animations** - Smooth animations and interactive 3D elements
- 📥 **PDF Download** - Download a birthday card PDF directly from the site
- 🎮 **Interactive Controls** - Toggle music on/off with floating button
- 💾 **Session Persistence** - Uses localStorage to remember login state

## 🚀 Deployment Instructions

### Deploy to Vercel (Recommended)

1. **Push to GitHub:**
   ```bash
   git init
   git add .
   git commit -m "Initial commit - Birthday card website"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
   git push -u origin main
   ```

2. **Deploy to Vercel:**
   - Go to [vercel.com](https://vercel.com)
   - Click "New Project"
   - Import your GitHub repository
   - Vercel will automatically detect settings
   - Click "Deploy"
   - Your site will be live at `https://your-project.vercel.app`

### Deploy to GitHub Pages

1. **Push to GitHub** (same as above)

2. **Enable GitHub Pages:**
   - Go to your repository settings
   - Scroll to "Pages" section
   - Select `main` branch as source
   - Click Save
   - Your site will be live at `https://YOUR_USERNAME.github.io/YOUR_REPO`

3. **Important:** If using GitHub Pages, update the `vercel.json` routing or remove it.

## 📋 Login Credentials

**Question:** What is your best friend's name?  
**Valid Answers:** 
- `candee` (case-insensitive)
- `candy` (case-insensitive)

## 🎵 Audio Functionality

The website includes automatic music playback with these features:

- **Auto-play on Login:** Music starts automatically when user logs in successfully
- **Loop Playback:** Music plays continuously in a loop
- **Manual Control:** Floating button in top-right corner to pause/play music
- **Mobile Support:** Includes fallbacks for mobile browsers with strict auto-play policies
- **Volume Control:** Pre-set to 50% volume for comfortable listening

### Browser Auto-play Notes

Some browsers (especially mobile) block auto-play. The site handles this by:
1. Attempting auto-play on page load
2. If blocked, attempting on first user interaction
3. Showing a visual indicator (bouncing golden button) if user action is needed
4. Allowing manual control via the music toggle button

## 📁 File Structure

```
aqsa-main/
├── index.html              # Main birthday card page
├── login.html              # Login/authentication page
├── style.css               # All styling and animations
├── UDI UDI.mp3            # Background music file
├── Happy_Birthday_Noshi.pdf # Downloadable birthday card
├── images/                 # Image assets
│   ├── 1.png
│   ├── balloon1.png
│   ├── balloon2.png
│   ├── unnamed.png
│   └── ...
├── vercel.json            # Vercel deployment configuration
├── .gitignore             # Git ignore file
└── README.md              # This file
```

## 🛠️ Technical Details

- **No Build Process Required** - Pure HTML, CSS, and JavaScript
- **CDN Dependencies:**
  - jQuery 3.7.1
  - Font Awesome 6.5.1
  - Google Fonts (Dancing Script, Poppins)
  - Spline Runtime for 3D effects (login page)

## 🔧 Customization

### Change Login Password
Edit `login.html` line ~451:
```javascript
const VALID_ANSWERS = ["candee", "candy"]; // Add more answers here
```

### Change Background Music
Replace `UDI UDI.mp3` with your audio file and update the reference in `index.html`.

### Update Birthday Message
Edit the text content in `index.html` around line ~165.

## 📱 Browser Compatibility

- ✅ Chrome/Edge (Desktop & Mobile)
- ✅ Firefox (Desktop & Mobile)
- ✅ Safari (Desktop & Mobile)
- ✅ Opera
- ⚠️ Internet Explorer (not recommended)

## 🐛 Troubleshooting

### Music Not Playing?
1. Check browser console for errors
2. Ensure audio file exists and path is correct
3. Click the music toggle button manually
4. Check browser auto-play settings

### Login Not Working?
1. Clear localStorage: `localStorage.clear()` in browser console
2. Check browser console for JavaScript errors
3. Verify answer matches (case-insensitive)

### Images Not Loading?
1. Verify all image files exist in the `images/` folder
2. Check file paths in HTML are correct
3. Ensure proper file extensions

## 📄 License

This is a personal birthday card project. Feel free to use and modify for personal purposes.

## 💝 Credits

Created with love for Noshi's 17th birthday! 🎉

---

**Deployed with:** Vercel / GitHub Pages  
**Last Updated:** July 2026
