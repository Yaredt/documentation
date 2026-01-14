# MarketGuard Support Documentation

**Last Updated**: January 27, 2025

## Getting Help

If you need assistance with MarketGuard, you can:

- **Email**: [Your support email]
- **GitHub Issues**: [GitHub repository URL]/issues
- **Documentation**: Check this guide for common questions and solutions

## Installation

### Installing from Chrome Web Store

1. Visit the [MarketGuard Chrome Web Store page](https://chrome.google.com/webstore)
2. Click "Add to Chrome"
3. Confirm the installation
4. The extension will appear in your browser toolbar

### Installing for Development

1. Clone or download the MarketGuard repository
2. Build the extension: `cd extension && npm run build`
3. Open Chrome and navigate to `chrome://extensions/`
4. Enable "Developer mode" (toggle in top right)
5. Click "Load unpacked"
6. Select the `extension/dist` directory

## Getting Started

### First-Time Setup

1. **Install the Extension**: Install MarketGuard from Chrome Web Store
2. **Visit Facebook Messenger**: Navigate to a Marketplace conversation
3. **Automatic Activation**: The extension automatically activates when you view Messenger conversations
4. **View Lead Scores**: Lead scores appear as overlays on buyer messages
5. **Check Risk Flags**: Scam detection warnings appear for suspicious messages

### Authentication

MarketGuard requires authentication to connect to the backend API:

1. Click the MarketGuard extension icon in your browser toolbar
2. Click "Sign In" or "Login"
3. Choose authentication method:
   - **Email/Password**: Create an account or sign in
   - **Facebook OAuth**: Sign in with your Facebook account
4. Once authenticated, the extension will connect to the backend API

## Features

### Lead Scoring

**What it does**: Analyzes buyer messages to provide a lead score (0-100) indicating buying intent.

**How to use**:
- Lead scores appear automatically as overlays on buyer messages
- Higher scores indicate stronger buying intent
- Click on a score to see detailed analysis

**Understanding scores**:
- **80-100**: High intent - likely to purchase
- **60-79**: Medium intent - interested but may need more information
- **40-59**: Low intent - casual inquiry
- **0-39**: Very low intent - may not be serious buyer

### Scam Detection

**What it does**: Identifies potential scam patterns in buyer messages.

**How to use**:
- Risk flags appear automatically on suspicious messages
- Red flags indicate high risk
- Yellow flags indicate moderate risk
- Click on a flag to see detected patterns

**Common scam patterns detected**:
- Requests for personal information
- Suspicious payment methods
- Urgent or pressure tactics
- Unusual communication patterns

### Draft Reply Generation

**What it does**: Generates suggested reply drafts based on conversation context.

**How to use**:
1. View a conversation in Facebook Messenger
2. Click the "Generate Reply" button (if available)
3. Review the suggested draft
4. Edit as needed before sending
5. **Important**: You must manually send the reply - the extension never sends messages automatically

## Troubleshooting

### Extension Not Working

**Symptoms**: Extension doesn't appear or doesn't analyze conversations

**Solutions**:
1. **Refresh the page**: Reload Facebook Messenger
2. **Check extension is enabled**: Go to `chrome://extensions/` and verify MarketGuard is enabled
3. **Check permissions**: Ensure the extension has permission to access Facebook and Messenger
4. **Restart browser**: Close and reopen Chrome
5. **Reinstall extension**: Remove and reinstall from Chrome Web Store

### Lead Scores Not Appearing

**Symptoms**: Messages don't show lead score overlays

**Solutions**:
1. **Check authentication**: Ensure you're logged in to MarketGuard
2. **Check backend connection**: Verify the backend API is accessible
3. **Check console for errors**: Open browser DevTools (F12) and check Console tab
4. **Verify conversation format**: Ensure you're viewing a Marketplace conversation

### Backend Unavailable

**Symptoms**: Extension shows "Backend unavailable" error

**Solutions**:
1. **Check internet connection**: Ensure you have internet access
2. **Check backend status**: Visit the backend health endpoint
3. **Wait and retry**: Backend may be temporarily unavailable
4. **Check extension settings**: Verify API URL is correct

### Authentication Issues

**Symptoms**: Can't log in or authentication fails

**Solutions**:
1. **Check credentials**: Verify email/password are correct
2. **Try Facebook OAuth**: Use Facebook login as alternative
3. **Clear extension data**: Go to `chrome://extensions/` → MarketGuard → Details → Clear storage
4. **Re-authenticate**: Sign out and sign back in

### Permission Errors

**Symptoms**: Extension requests permissions or shows permission errors

**Solutions**:
1. **Grant permissions**: Click "Allow" when Chrome prompts for permissions
2. **Check host permissions**: Ensure Facebook and Messenger URLs are allowed
3. **Review permissions**: Go to `chrome://extensions/` → MarketGuard → Details → Permissions

## Common Questions

### Is my data secure?

Yes. MarketGuard uses encryption for all data transmission and follows industry-standard security practices. See our [Privacy Policy](../docs/PRIVACY_POLICY.md) for details.

### Does the extension send messages automatically?

**No**. MarketGuard never sends messages automatically. All actions require your explicit confirmation. The extension only provides analysis and suggestions.

### Can I use MarketGuard without internet?

No. MarketGuard requires internet connection to communicate with the backend API for analysis. Some basic features may work offline, but lead scoring and scam detection require API access.

### Does MarketGuard work on mobile?

MarketGuard is a Chrome extension and works on desktop Chrome browsers. It does not work on mobile Chrome or other browsers.

### How do I uninstall MarketGuard?

1. Go to `chrome://extensions/`
2. Find MarketGuard in the list
3. Click "Remove"
4. Confirm removal

**Note**: Uninstalling removes locally stored data. Backend data can be deleted by contacting support.

### Can I export my data?

Yes. You can export your conversation analysis data through the Extension settings. Contact support for account data export.

### How do I report a bug?

Report bugs by:
- Opening a GitHub Issue: [GitHub repository URL]/issues
- Emailing support: [Your support email]
- Include: Browser version, extension version, steps to reproduce, error messages

### How do I request a feature?

Feature requests can be submitted:
- Via GitHub Issues: [GitHub repository URL]/issues
- Via email: [Your support email]

## Privacy and Data

### What data does MarketGuard collect?

MarketGuard collects:
- Conversation messages (for analysis)
- User preferences (stored locally)
- Authentication tokens (stored locally)
- Usage statistics (for improvement)

See our [Privacy Policy](../docs/PRIVACY_POLICY.md) for complete details.

### How long is my data stored?

- Conversation data: 90 days
- User preferences: Until you delete your account
- Authentication tokens: Until you log out

### Can I delete my data?

Yes. You can:
- Delete locally stored data by uninstalling the extension
- Request backend data deletion by contacting support
- Delete your account through extension settings

## Technical Requirements

### Browser Compatibility

- **Chrome**: Version 88 or later
- **Chromium-based browsers**: May work but not officially supported
- **Other browsers**: Not supported

### System Requirements

- Internet connection required
- JavaScript enabled
- Chrome extensions enabled

## Updates

### How are updates delivered?

Updates are automatically delivered through Chrome Web Store. You don't need to do anything - Chrome will update the extension automatically.

### How do I check my extension version?

1. Go to `chrome://extensions/`
2. Find MarketGuard
3. Version number is displayed under the extension name

## Contact Support

For additional help:

- **Email**: [Your support email]
- **GitHub Issues**: [GitHub repository URL]/issues
- **Documentation**: [Your documentation URL]

We aim to respond to support requests within 48 hours.

---

**Note**: This support documentation is provided to help users get the most out of MarketGuard. For privacy concerns, see our [Privacy Policy](../docs/PRIVACY_POLICY.md).
