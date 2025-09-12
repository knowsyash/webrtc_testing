# WebRTC Video Call Demo

A simple WebRTC video calling application that uses Firebase Realtime Database for signaling.

## Features

- Create a video call with a shareable 6-character ID
- Join calls using the ID
- Real-time video and audio communication
- Works across different computers/networks
- Easy-to-use interface with copy functionality

## How to Deploy to GitHub Pages

### Step 1: Create a GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the "+" icon and select "New repository"
3. Name your repository (e.g., "webrtc-video-call")
4. Make sure it's set to "Public"
5. Check "Add a README file"
6. Click "Create repository"

### Step 2: Upload Your Files

1. Click "uploading an existing file" or drag and drop
2. Upload your `index.html` file
3. Add a commit message like "Add WebRTC video call app"
4. Click "Commit changes"

### Step 3: Enable GitHub Pages

1. In your repository, go to **Settings** (top menu)
2. Scroll down to **Pages** (left sidebar)
3. Under "Source", select **"Deploy from a branch"**
4. Choose **"main"** branch and **"/ (root)"** folder
5. Click **Save**
6. GitHub will provide you with a URL like: `https://yourusername.github.io/your-repo-name`

### Step 4: Wait and Test

1. Wait 2-5 minutes for GitHub Pages to deploy
2. Visit your GitHub Pages URL
3. The app should be live!

## How to Test the Video Call

### Testing with Two Computers:

1. **Computer 1 (Call Creator):**
   - Open your GitHub Pages URL
   - Click "Create New Call"
   - Allow camera/microphone permissions
   - A 6-character Call ID will be generated
   - Copy the Call ID and share it

2. **Computer 2 (Call Joiner):**
   - Open the same GitHub Pages URL
   - Enter the Call ID in the "Join a Call" field
   - Click "Join Call"
   - Allow camera/microphone permissions
   - You should now see both video feeds!

### Testing on the Same Computer (for initial testing):

1. Open two different browser tabs or use different browsers
2. Follow the same steps as above
3. You'll see your own video in both windows

## Troubleshooting

### Camera/Microphone Not Working:
- Make sure you click "Allow" when the browser asks for permissions
- Try refreshing the page and trying again
- Check your browser settings for camera/microphone permissions

### Call Not Connecting:
- Make sure both people are using the exact same Call ID
- Check that both people have allowed camera/microphone permissions
- Try refreshing both pages and starting over
- Make sure you're both using the same GitHub Pages URL

### Firebase Issues:
- The app uses a pre-configured Firebase database
- If you want to use your own Firebase project, you'll need to:
  1. Create a Firebase project
  2. Enable Realtime Database
  3. Replace the Firebase config in the HTML file

## Browser Compatibility

This app works best with:
- Chrome (recommended)
- Firefox
- Safari
- Edge

**Note:** WebRTC requires HTTPS or localhost to work properly. GitHub Pages automatically provides HTTPS, which is why it's perfect for this app!

## Security Note

The Firebase configuration is visible in the code, which is normal for client-side applications. The database is configured with security rules to only allow WebRTC signaling data.