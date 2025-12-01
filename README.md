# CF Training Analytics - Professional Progress Tracker

A beautiful, GitHub-inspired Codeforces training tracker with Firebase cloud sync. Track your daily problem-solving progress across multiple devices with real-time synchronization.

![CF Training Analytics](https://img.shields.io/badge/Status-Active-success)
![License](https://img.shields.io/badge/License-MIT-blue)
![Firebase](https://img.shields.io/badge/Firebase-Enabled-orange)

## 🌟 Live Demo

**Access the tracker here:** [https://cthboss001.github.io/pupil](https://cthboss001.github.io/pupil)

## ✨ Features

### 📊 Progress Tracking
- **Daily Problem Tracking** - Mark problems solved for three rating categories (1000, 1100, 1200)
- **Beautiful Heatmap** - GitHub-style contribution graph showing your activity
- **Streak Counter** - Track current and longest solving streaks
- **Statistics Dashboard** - View completion rates and moving averages

### ☁️ Cloud Sync
- **Firebase Integration** - Automatic cloud backup and synchronization
- **Multi-Device Support** - Access your data from phone, tablet, and desktop
- **Real-Time Updates** - Changes sync across devices within seconds
- **Offline Capable** - Works without internet, syncs when back online

### 🎨 Professional Design
- **GitHub-Inspired UI** - Dark theme with professional aesthetics
- **Responsive Layout** - Optimized for mobile and desktop
- **Smooth Animations** - Confetti celebrations on achievements
- **Touch-Friendly** - Easy to use on mobile devices

### 🔒 Data Management
- **Local Storage** - Fast, instant saves
- **Export/Import** - Download JSON backups
- **Auto-Cleanup** - Configurable data retention
- **PIN Lock** - Optional security (can be disabled)

## 🚀 Quick Start

### 1. Access the Tracker
Open [https://cthboss001.github.io/pupil](https://cthboss001.github.io/pupil) in your browser.

### 2. Optional: Set Up Firebase Sync
For cross-device synchronization:

1. Create a Firebase project at [Firebase Console](https://console.firebase.google.com)
2. Enable **Realtime Database**
3. Set database rules to test mode:
   ```json
   {
     "rules": {
       "users": {
         "$uid": {
           ".read": true,
           ".write": true
         }
       }
     }
   }
   ```
4. Get your Firebase configuration from Project Settings
5. In the tracker, click **"🔥 Firebase Setup"**
6. Enter your credentials and a unique User ID
7. Click **"Save & Connect"**

### 3. Start Tracking!
- Mark checkboxes for each rating (1000, 1100, 1200) as you solve problems
- Watch your stats grow and streaks build!

## 📱 Mobile Usage

### Add to Home Screen (PWA-like experience)

**iPhone:**
1. Open tracker in Safari
2. Tap Share button
3. Select "Add to Home Screen"
4. Tap "Add"

**Android:**
1. Open tracker in Chrome
2. Tap three-dot menu
3. Select "Add to Home screen"
4. Tap "Add"

Now access it like a native app from your home screen!

## 🎯 Daily Workflow

```
Morning:
  ☕ Open tracker
  👀 See today's goal: 0/3 problems

After Solving on Codeforces:
  ✅ Mark Rating 1000
  🎉 Confetti animation!
  ☁️ Auto-syncs to cloud

Continue Throughout Day:
  ✅ Mark Rating 1100
  ✅ Mark Rating 1200
  🎊 All 3 complete! Streak continues!

Evening:
  📊 Review stats
  📈 Check heatmap
  🔥 Admire your streak
```

## ⚙️ Settings

Access via **⚙️ Settings** button:

- **Data Retention**: How long to keep old records (default: 365 days)
- **Days to Display**: Number of days shown in heatmap (default: 60)
- **Daily Reminder**: Set notification time
- **Animations**: Toggle confetti effects
- **PIN Lock**: Optional 4-digit security (leave blank to disable)

## 🔧 Features Explained

### Stats Overview
- **Rating Cards**: Problems solved per rating category
- **Current Streak**: Consecutive days with at least 1 problem solved
- **Longest Streak**: Your personal best
- **Total Solved**: All-time problem count

### Activity Heatmap
- **GitHub-style visualization** of your daily activity
- **Color intensity** shows problems solved per day
- **Hover** to see exact dates and counts
- **Scrollable** to view full history

### Analytics
- **Completion Rate**: Percentage of days you solved each rating
- **Moving Averages**: 7, 14, 30-day performance trends
- **Activity Chart**: Visual graph of recent progress

### Data Management
- **Export**: Download JSON backup of all data
- **Import**: Restore from previous backup
- **Clear Old Data**: Remove records older than retention period

## 🔑 Keyboard Shortcuts

- **Ctrl + Z**: Undo last action
- **Ctrl + Y**: Redo action

## 🛠️ Tech Stack

- **Frontend**: Pure HTML, CSS, JavaScript (no frameworks!)
- **Storage**: LocalStorage + Firebase Realtime Database
- **Design**: GitHub-inspired design system
- **Hosting**: GitHub Pages (free!)
- **CDN**: Firebase SDK via CDN

## 📦 Self-Hosting

Want to host your own version?

1. **Fork this repository**
2. **Edit `index.html`** if you want customizations
3. **Enable GitHub Pages**:
   - Go to Settings → Pages
   - Select `main` branch
   - Save
4. **Access at**: `https://yourusername.github.io/pupil`

## 🔒 Privacy & Data

- **Your data stays yours**: Stored in your browser and your Firebase project
- **No tracking**: No analytics or third-party scripts
- **No backend**: All processing happens client-side
- **Open source**: Inspect the code yourself!

## 🐛 Troubleshooting

### Firebase Not Syncing?
1. Check if credentials are entered on all devices
2. Verify User ID is identical on all devices
3. Check Firebase Console to see if data appears
4. Clear browser cache and reconfigure

### Data Not Showing on Mobile?
1. Enter Firebase credentials on mobile
2. Use the same User ID as desktop
3. Refresh the page
4. Check sync indicator (should show "Synced")

### PIN Popup Annoying?
Remove it via:
```javascript
// Open browser console (F12) and run:
dataManager.data.pinHash = null;
dataManager.save();
location.reload();
```

### Heatmap Not Loading?
1. Refresh the page
2. Check browser console for errors
3. Try a different browser
4. Clear cache

## 🤝 Contributing

Contributions welcome! Feel free to:
- Report bugs
- Suggest features
- Submit pull requests
- Share feedback

## 📄 License

MIT License - Free to use, modify, and distribute!

## 💬 Support

Questions or issues? Open an issue in this repository!

## 🎉 Acknowledgments

- Inspired by GitHub's contribution graph
- Built for the Codeforces competitive programming community
- Designed with senior engineering standards in mind

---

**Start tracking your progress today!** 🚀

[Open Tracker](https://cthboss001.github.io/pupil) | [Report Issue](https://github.com/cthboss001/pupil/issues)

---

Made with ❤️ for competitive programmers
