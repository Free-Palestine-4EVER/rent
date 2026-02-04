# More Rent A Car - iOS App

## Building on Mac

### Prerequisites
1. macOS with Xcode installed (from App Store)
2. Node.js installed
3. Apple Developer account (for App Store submission)

### Build Steps

```bash
# 1. Install dependencies (if not already done)
npm install

# 2. Sync Capacitor (copies latest web files to iOS)
npx cap sync ios

# 3. Open in Xcode
npx cap open ios
```

### In Xcode

1. **Select your team** in Signing & Capabilities
2. **Update Bundle Identifier** if needed (currently: `com.morerentcar.app`)
3. **Select a device** or simulator
4. **Press Play (⌘R)** to run

### App Icons

The main 1024x1024 icon is included. Use an icon generator tool to create all sizes:
- [AppIconGenerator.com](https://appicon.co/)
- Upload `AppIcon-1024.png` and download the complete set

### TestFlight / App Store

1. In Xcode: **Product → Archive**
2. Open **Organizer** (Window → Organizer)
3. Click **Distribute App**
4. Follow the prompts to upload to App Store Connect

## Features

- 📱 Native iOS app with web content
- 📷 Camera access for license verification
- 🔒 Secure identity verification with OCR
- 🚗 All 11 luxury vehicles
- 💰 Live price calculator

## Files Structure

```
ios/
├── App/
│   ├── App/
│   │   ├── Info.plist (camera permissions)
│   │   └── Assets.xcassets/ (icons)
│   ├── App.xcodeproj
│   └── CapApp-SPM/
www/
├── index.html
├── cars.html
├── contact.html
└── images/
```
