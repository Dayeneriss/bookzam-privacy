# Privacy Policy — BookZam

Last updated: April 2, 2026

BookZam respects your privacy. This policy explains what data is collected, how it is used, and your rights.

## 1. Data Collected

### 1.1 Account Data
- Email address and name (when creating an account)
- Login identifier via Google Sign-In or Sign in with Apple
- Profile photo (if provided via Google or Apple)

### 1.2 Library Data
- History of scanned, searched, and added books
- Favorites, personal notes, reading statuses
- Reading progress and goals
- Reading challenges and badges earned

### 1.3 Listening Data (Audiobooks)
- Listening sessions (start, end, duration, playback speed)
- Progress per chapter and per audiobook
- Post-listening feedback (abandonment or completion)

### 1.4 Social Data
- Public profile: username, reading level, preferred genres, book count, badges
- Shared activity: books added, challenges completed, badges earned
- Messages in book clubs

### 1.5 AI-Related Data
When you use artificial intelligence features (mood search, quote search, Book DNA, Forgotten Book chat, quiz, recommendations), the text you enter along with your library context is sent to Google servers (Gemini) for processing. No cover images are sent for text recognition (OCR), which is performed entirely on your device.

### 1.6 Technical Data
- Device model, operating system version, app version
- Anonymous crash logs (error traces, without personal data)
- Anonymized usage events (screens visited, features used)
- Push notification token (FCM token)

### 1.7 Location Data
- Approximate geographic location (only if you authorize it), used to redirect you to the correct Amazon store for your country. This data is not stored on our servers.

### 1.8 Media Data
- Camera access (to scan book covers and shelves)
- Photo access (to select book images)
- Microphone access (for voice search)
- This data is processed locally or transmitted temporarily for recognition. It is not stored on our servers.

## 2. Use of Data

- Provide core app features (library, search, recommendations, audiobooks, quizzes, book clubs)
- Personalize your experience (AI recommendations, Book DNA, reading profile)
- Manage your Premium subscription
- Display relevant ads (for free users only)
- Improve the application (anonymized usage statistics, bug fixes)
- Send reminder and progress notifications (can be disabled in settings)
- **No data is sold to third parties**

## 3. Third-Party Services

BookZam uses the following third-party services:

| Service | Purpose | Data Transmitted |
|---------|---------|------------------|
| **Firebase Authentication** | Secure sign-in | Email, name, login ID |
| **Cloud Firestore** | Data storage | Library, profile, progress |
| **Firebase Analytics** | Usage statistics | Anonymized events, user properties |
| **Firebase Crashlytics** | Crash reports | Error traces, device info |
| **Firebase Cloud Messaging** | Push notifications | FCM token |
| **Firebase Remote Config** | Dynamic configuration | No personal data |
| **Firebase App Check** | Fraud protection | Device attestation |
| **Google Generative AI (Gemini)** | AI features | Search text, library context |
| **RevenueCat** | Subscription management | User ID, subscription status |
| **Google AdMob** | Advertising | Advertising ID (GAID/IDFA) |
| **Google Books API** | Book search | Search terms (title, author, ISBN) |
| **Open Library** | Book search | Search terms |
| **Library of Congress** | Book search (fallback) | Search terms |
| **LibriVox** | Free audiobooks | Title, author |
| **Google ML Kit** | OCR (on-device) | None — local processing only |

When comparative testing (shadow testing) is enabled, your AI queries may also be processed by Anthropic (Claude) alongside Gemini.

## 4. Storage and Security

- Data is stored on **Google Firebase** (secure infrastructure, encryption in transit and at rest)
- Local data (cache, preferences) is stored on your device via SharedPreferences and sqflite (unencrypted)
- Images captured by the camera are temporarily stored on your device and are not sent to our servers (except for shelf analysis via Gemini Vision, when applicable)

## 5. Advertising

- **Free** users see banner ads provided by Google AdMob
- Users can watch **rewarded ads** to earn additional AI searches
- **Premium** users see no ads
- Google AdMob may collect advertising identifiers (GAID on Android, IDFA on iOS) to personalize ads
- On iOS, a consent prompt (App Tracking Transparency) will be presented before any advertising identifier is collected

## 6. Notifications

- BookZam may send push notifications for reading reminders, reading streaks, challenges, recommendations, and updates
- You can disable each notification category individually in the app settings
- You can unsubscribe from notifications entirely at any time

## 7. Public Profile and Social Data

- Some profile information is visible to other users: username, reading level, preferred genres, book count, badges
- The activity feed (books added, challenges completed, badges) is visible to all logged-in users
- Book club messages are visible to club members
- You can control your profile visibility in the settings

## 8. User Rights

In accordance with GDPR and applicable laws, you may:
- **Access** your personal data
- **Rectify** your information
- **Delete** your account and all your data
- **Export** your data upon request
- **Withdraw your consent** for notifications and location via the app settings

To exercise these rights, contact us at **contact@bookzam.io**

## 9. Data Retention

- Your account data is retained as long as your account is active
- Upon account deletion, your data is erased within 30 days
- Crash logs are retained for 90 days
- Analytics events are retained according to Firebase's retention policy (14 months by default)

## 10. Children

BookZam is not intended for children under 13 years of age. We do not knowingly collect personal data from children. If you are a parent and believe your child has provided us with data, contact us at contact@bookzam.io.

## 11. Changes

BookZam may update this policy. In case of major changes, we will inform you via the app or by email. The last update date is shown at the top of this document.

## 12. Contact

For any questions or requests regarding your data:
- Email: **contact@bookzam.io**
- You can also use the feedback feature in the app (Settings > Feedback)
