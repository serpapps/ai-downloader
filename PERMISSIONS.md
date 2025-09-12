# Permissions Justification for AI Downloader

We believe in transparency and minimal permissions. AI Downloader only requests the permissions absolutely necessary for core functionality. This document provides detailed explanations for each permission and how it's used.

## Our Privacy Commitment

- **Privacy First**: No data tracking, no analytics, no personal information collection
- **Local Processing**: All AI processing happens on your device
- **Minimal Permissions**: Only essential permissions for core functionality
- **Transparent**: Complete documentation of why each permission is needed

## Desktop Application Permissions

### File System Access
**Why it's needed**: Save downloaded media files to your computer in locations you choose.
**How it's used**: 
- Write downloaded videos, audio, images, and documents to selected folders
- Create organized folder structures based on AI categorization
- Read configuration files and user preferences
- Cache AI models and temporary processing files

**What we don't do**: Access files unrelated to AI Downloader functionality or browse your personal files without explicit user action.

### Network/Internet Access
**Why it's needed**: Download media content from websites and online platforms.
**How it's used**:
- Connect to websites and platforms to detect and download media
- Fetch metadata and thumbnails for media content
- Download AI models and updates (optional, user-controlled)
- Check for application updates (optional, can be disabled)

**What we don't do**: Send personal data, browsing history, or downloaded content to our servers.

### System Resources (CPU, Memory)
**Why it's needed**: Run AI processing for content detection, optimization, and organization.
**How it's used**:
- Execute AI models for media detection and analysis
- Process and optimize downloaded content (format conversion, compression)
- Manage multiple concurrent downloads efficiently
- Organize and categorize content using machine learning

**What we don't do**: Mine cryptocurrency, run background processes when app is closed, or consume excessive resources.

## Browser Extension Permissions

### activeTab
**Why it's needed**: Analyze the currently open webpage to detect downloadable media.
**How it's used**:
- Scan the active browser tab for videos, images, audio, and documents
- Extract metadata and quality information for detected media
- Only activates when you click the extension icon

**What we don't do**: Monitor your browsing activity or access tabs you're not actively using the extension on.

### downloads
**Why it's needed**: Initiate and manage file downloads through the browser's download system.
**How it's used**:
- Start downloads of detected media files
- Track download progress and handle interruptions
- Integrate with browser's download manager for user visibility

**What we don't do**: Download files without explicit user permission or access downloads from other applications.

### storage
**Why it's needed**: Store user preferences, settings, and temporary AI processing data.
**How it's used**:
- Save your download preferences and quality settings
- Cache AI model data for improved performance
- Store temporary processing data for batch operations
- Remember user interface customizations

**What we don't do**: Store personal information, browsing history, or share stored data with external services.

### tabs
**Why it's needed**: Detect when you navigate to pages with downloadable content.
**How it's used**:
- Identify when you're on supported platforms (YouTube, Vimeo, etc.)
- Show the extension icon when downloadable content is available
- Enable automatic content detection on supported sites

**What we don't do**: Track your browsing history or monitor tabs unrelated to media downloading.

### scripting
**Why it's needed**: Execute AI detection algorithms and content analysis scripts on web pages.
**How it's used**:
- Run AI models to detect media content on complex websites
- Extract video/audio stream URLs from JavaScript variables
- Analyze page structure to find hidden download links

**What we don't do**: Modify website content, inject ads, or run scripts for purposes other than media detection.

### cookies
**Why it's needed**: Access authentication cookies to download private or user-specific content.
**How it's used**:
- Access content from platforms where you're logged in (private videos, purchased courses)
- Maintain session state for platforms that require authentication
- Download content that requires user-specific permissions

**What we don't do**: Access cookies from unrelated websites or share authentication information.

### host_permissions
**Why it's needed**: Access specific website domains to detect and download media content.
**How it's used**:
- Connect to supported platforms (YouTube, TikTok, Vimeo, etc.) for media detection
- Access CDNs and media servers to download content
- Fetch metadata and thumbnails from various domains

**Specific domains we access**:
- Video platforms: youtube.com, vimeo.com, tiktok.com, instagram.com
- CDN networks: Various content delivery networks used by platforms
- Media servers: Direct video/audio stream servers

**What we don't do**: Access domains unrelated to media downloading or track users across websites.

### contextMenus
**Why it's needed**: Add convenient right-click options for quick media downloading.
**How it's used**:
- Add "Download with AI Downloader" to right-click menus on media elements
- Provide quick access to download options for links and embedded content
- Enable batch selection through context menu actions

**What we don't do**: Modify existing browser context menus or add irrelevant menu items.

### notifications
**Why it's needed**: Inform users about download progress, completion, and any issues.
**How it's used**:
- Notify when downloads start, complete, or encounter errors
- Show progress updates for long-running batch operations
- Alert users to important status changes or AI processing updates

**What we don't do**: Send promotional notifications, ads, or notifications unrelated to current downloads.

### webNavigation
**Why it's needed**: Monitor navigation to automatically enable AI detection on supported sites.
**How it's used**:
- Detect when you visit supported platforms for automatic content scanning
- Enable context-appropriate features based on the current website
- Optimize AI models based on the type of content detected

**What we don't do**: Track complete browsing history or monitor navigation to unrelated websites.

## Advanced Features Permissions

### offscreen (Browser Extension)
**Why it's needed**: Process complex media analysis and AI computations in background threads.
**How it's used**:
- Run intensive AI models without blocking the browser interface
- Process large batch downloads efficiently
- Handle format conversions and optimizations in the background

**What we don't do**: Run unnecessary background processes or consume resources when not actively downloading.

### clipboardRead (Optional)
**Why it's needed**: Allow users to quickly paste URLs for immediate download analysis.
**How it's used**:
- Read URLs from clipboard when users use "paste URL" feature
- Enable quick workflows for batch URL processing
- Only activated with explicit user action (clicking paste button)

**What we don't do**: Continuously monitor clipboard contents or access clipboard data without user interaction.

## Data Collection and Privacy

### What We Collect: NOTHING
- **No personal information** is collected or stored on our servers
- **No browsing history** is tracked or recorded
- **No download history** is sent to external services
- **No usage analytics** are gathered or transmitted
- **No AI training data** is collected from user activities

### What Stays Local
- All downloaded content remains on your device
- AI models and processing happen locally
- User preferences and settings are stored locally
- Temporary processing files are cleaned up automatically

### Optional Data
- **Update checks**: Can be disabled in settings
- **Error reporting**: Completely optional and anonymous
- **Feature suggestions**: Only if explicitly submitted by user

## Third-Party Services

AI Downloader may connect to third-party services only for essential functionality:

### Platform APIs (Read-Only)
- **YouTube API**: For metadata and video information (no user data sent)
- **Vimeo API**: For video details and stream URLs (no personal information shared)
- **Other platform APIs**: Similar read-only access for supported platforms

### CDN Access
- **Media CDNs**: Direct connections to download content (standard HTTP requests)
- **No tracking**: These connections don't include user identification

### AI Model Updates (Optional)
- **Model downloads**: Improved AI models for better detection (can be disabled)
- **Anonymous**: No user data sent when downloading models

## Security Measures

### Data Protection
- **Encryption**: All local data storage is encrypted
- **Secure connections**: All network traffic uses HTTPS
- **Sandboxing**: AI processing is isolated from system access

### Safe Downloads
- **Virus scanning**: Downloaded files are checked for malware
- **Integrity verification**: Files are verified to match expected content
- **Safe defaults**: Conservative security settings enabled by default

## User Control

### Granular Permissions
- Enable/disable specific features and permissions
- Choose which platforms and content types to support
- Control AI processing levels and resource usage

### Complete Transparency
- View all network connections in real-time
- Monitor file system access and modifications
- Audit AI model usage and processing activities

### Easy Removal
- Complete uninstall removes all traces of the application
- No hidden files, registry entries, or background services
- User data deletion tools included

## Compliance

AI Downloader is designed to comply with:
- **GDPR**: No personal data collection, user control over all processing
- **CCPA**: No personal information sale or sharing
- **COPPA**: No data collection from users of any age
- **Platform Terms**: Respectful API usage and rate limiting

## Questions or Concerns?

If you have any questions about our permissions usage or privacy practices:

- 📧 **Email**: privacy@serpapps.com
- 💬 **Community**: [GitHub Discussions](https://github.com/orgs/serpapps/discussions)
- 🐛 **Issues**: [Report concerns](https://github.com/serpapps/ai-downloader/issues)

We're committed to transparency and will always explain our permissions usage in detail.

---

**Last Updated**: September 2024  
**Version**: 1.0