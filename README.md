# Awesome-Push-Notifications

## Top Push Notification Platforms & Tools

A curated list of leading platforms and frameworks for sending, managing, and optimizing push notifications across mobile, web, and multi-channel engagement.  
**Primary focus: open-source software.**

Commercial / hosted platforms are listed separately for completeness. Open-source alternatives and community tools are emphasized throughout.

---

## SaaS / Hosted Platforms

| Platform | Description | Key Focus |
|----------|-------------|-----------|
| **[OneSignal](https://onesignal.com/)** | Complete platform for push notifications across mobile, web, and desktop. Supports campaigns, Journeys, segmentation, A/B testing, personalization, and multi-channel messaging (push, email, SMS, in-app). | High-volume engagement, free tier for unlimited mobile push |
| **[Airship](https://www.airship.com/)** | Enterprise customer engagement platform with push, in-app messages, Message Center, SMS/MMS/RCS, email, Live Activities, and advanced orchestration. | Enterprise mobile engagement & multi-channel journeys |
| **[Pushwoosh](https://www.pushwoosh.com/)** | Omnichannel customer engagement platform supporting push, in-app, email, SMS, WhatsApp, and more. High throughput (up to 500k pushes/sec), segmentation, and AI-assisted campaigns. | Omnichannel messaging & high-volume delivery |
| **[WonderPush](https://www.wonderpush.com/)** | Developer-friendly push platform for web and mobile. Fast delivery (350k/sec), GDPR-compliant, full-featured from low pricing, with automation, segmentation, and A/B testing. | Affordable full-featured push for web + mobile |
| **[Firebase Cloud Messaging (FCM)](https://firebase.google.com/products/cloud-messaging)** | Google’s free, reliable messaging service for iOS, Android, and web. Supports topics, device targeting, data messages, and integration with Analytics/A/B testing. | Free transport layer & Android-native push |
| **[MoEngage](https://www.moengage.com/)** | Customer engagement platform with AI-powered personalized push, rich media, Notification Center, event-triggered campaigns, and multi-channel orchestration. | AI-driven personalization & lifecycle campaigns |
| **[CleverTap](https://clevertap.com/)** | Retention and engagement platform with powerful segmentation, real-time triggers, rich push, Notification Inbox, and detailed analytics. | User retention & behavior-based campaigns |
| **[Braze](https://www.braze.com/)** | Customer engagement platform focused on personalized, cross-channel messaging including rich push, Intelligent Timing, Canvas journeys, and deep analytics. | Enterprise personalization & omnichannel journeys |
| **[Iterable](https://iterable.com/)** | Growth marketing platform with push (standard + silent), journeys, segmentation, and multi-channel orchestration (email, SMS, push, in-app). | Cross-channel journeys & growth marketing |
| **[WebEngage](https://webengage.com/)** | Full-stack customer engagement platform supporting mobile/web push, in-app, email, SMS, and WhatsApp with real-time segmentation and journey builders. | Omnichannel engagement & personalization |

---

## Open-Source Softwares

These tools form the core ecosystem for self-hosted, privacy-focused, or developer-controlled push notification systems. Most can integrate with APNs, FCM, or act as independent delivery layers.

### Core Frameworks & Servers

| Project | Description | License | Notes |
|---------|-------------|---------|-------|
| **[ntfy](https://github.com/binwiederhier/ntfy)** | Lightweight HTTP pub/sub push notification server. Publish via simple PUT/POST; clients receive on Android, iOS, web, or desktop. Supports UnifiedPush, priorities, attachments, and action buttons. | Apache 2.0 / GPL 2.0 | Best overall self-hosted option; public instance at ntfy.sh |
| **[Gotify](https://github.com/gotify/server)** | Simple self-hosted server for sending/receiving real-time messages via REST + WebSocket. Includes web UI, Android app, application tokens, and plugin system. | MIT | Lightweight, excellent for private notifications |
| **[Novu](https://github.com/novuhq/novu)** | Open-source notification infrastructure platform. Unified API for push, email, SMS, in-app, and chat with workflows, templates, digests, and subscriber preferences. | MIT (Open Core) | Dominant multi-channel open-source solution |
| **[UnifiedPush](https://unifiedpush.org/)** | Decentralized open standard and protocol for push notifications on Android (and beyond) without relying on Google FCM. Multiple distributors available. | Various open licenses | Privacy-focused FCM alternative |
| **[Apprise](https://github.com/caronc/apprise)** | Notification library that can push to 100+ services (Slack, Discord, Telegram, email, SMS, push services, etc.) from a single API. | BSD 3-Clause | Best as a multi-service relay / fan-out tool |
| **[Centrifugo](https://github.com/centrifugal/centrifugo)** | Scalable real-time messaging server with WebSockets, SSE, gRPC. Often used for live notifications, presence, and pub/sub. | Apache 2.0 | Strong for real-time / in-app notification fan-out |

### Specialized Libraries & Platforms

| Project | Description | Focus Area |
|---------|-------------|------------|
| **[Alô](https://github.com/butialabs/alo)** | Open-source alternative to OneSignal / PushNews-style platforms. Web push management, campaigns, analytics, and user segmentation. | Web push + campaigns |
| **[Notifo](https://github.com/notifo-io/notifo)** | Multi-channel notification service with REST API, management UI, templates, and support for email, web, push, and SMS. | Multi-channel self-hosted |
| **[Dittofeed](https://github.com/dittofeed/dittofeed)** | Developer-focused platform for automated omnichannel messaging (email, SMS, push, WhatsApp) with low-code journeys and segmentation. | Journeys & automation |
| **[Laudspeaker](https://github.com/laudspeaker/laudspeaker)** | Open-source customer engagement / messaging platform with journeys and multi-channel support. | Customer engagement |
| **[Expo Push Notifications](https://docs.expo.dev/push-notifications/overview/)** | Free unified push API (especially popular with React Native / Expo apps) that abstracts APNs and FCM. | React Native / Expo apps |
| **[Firebase Admin SDKs + FCM](https://firebase.google.com/docs/cloud-messaging)** | Official open client/server libraries (while the service itself is hosted). Widely used as the transport layer. | Android / cross-platform transport |

### Additional Notable Open-Source Tools

- **[Svix](https://github.com/svix/svix-webhooks)** – Open-source webhook infrastructure (often paired with push systems).
- **[AirNotifier](https://github.com/airnotifier/airnotifier)** – Self-hosted push notification server supporting multiple providers.
- **[PushSharp](https://github.com/Redth/PushSharp)** – Classic .NET library for multi-platform push (APNs, FCM, etc.).
- **[node-apn / node-gcm / web-push](https://github.com/web-push-libs)** – Popular Node.js libraries for APNs, FCM, and Web Push.
- **[pywebpush / pyfcm](https://github.com/web-push-libs)** – Python equivalents for Web Push and FCM.
- **[UnifiedPush distributors](https://unifiedpush.org/users/distributors/)** – ntfy, NextPush, and others that implement the UnifiedPush protocol.
- **[Matrix / Element notifications](https://matrix.org/)** – Can be leveraged for decentralized real-time notifications.
- **[Rocket.Chat / Mattermost notification integrations](https://github.com/RocketChat)** – Self-hosted chat platforms with strong push capabilities.

---

## Quick Start Recommendations

| Goal | Recommended Starting Point |
|------|---------------------------|
| Simple self-hosted personal/team alerts | **ntfy** or **Gotify** |
| Full multi-channel product notifications (push + email + SMS + in-app) | **Novu** |
| Privacy-focused Android push (no Google FCM) | **UnifiedPush** + ntfy |
| Web push only (self-hosted) | **Alô** or **web-push** libraries |
| React Native / Expo apps | **Expo Push** or **OneSignal** free tier |
| High-volume free transport layer | **Firebase Cloud Messaging (FCM)** |
| Multi-service fan-out (Slack, Discord, Telegram, etc.) | **Apprise** |
| Enterprise-grade SaaS with advanced journeys | **Braze**, **MoEngage**, or **CleverTap** |
| Lightweight real-time messaging | **Centrifugo** |

---

## Contributing

Contributions, corrections, and new open-source projects are welcome.  
Please open an issue or pull request.

---

**Last updated:** August 2026  
Emphasizing open-source tools while documenting the major commercial platforms for context.
