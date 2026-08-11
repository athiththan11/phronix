---
layout: default
title: Delete Account — Phronix
---

# Account Deletion Request

**App:** Phronix  
**Developer:** athiththan11

If you would like to delete your Phronix account and all associated data, follow the steps below.

---

## How to delete your account

### Option 1 — Delete directly in the app (recommended)

1. Open the **Phronix** app and sign in.
2. Tap **Profile** (bottom navigation bar).
3. Tap **Delete account**.
4. Confirm in the dialog that appears. This step is permanent and cannot be undone.

This immediately deletes your account (Firebase Authentication record), your synced cards, saved offers, favourite merchants, and settings (Cloud Firestore), and clears the app's local data on your device. If you signed in a while ago, you may be asked to sign in again — with whichever of Google or Apple you originally used — before the deletion can complete; this is a Firebase security requirement, not an extra step we added.

### Option 2 — Email request

If you no longer have access to the app, send a deletion request to **athiththan.kathir@gmail.com** with the subject line:

> Phronix — Account Deletion Request

Include the email address associated with your Phronix account. We will remove your account and all associated data from our active systems within **30 calendar days**.

---

## What data is deleted

| Data | Action |
|---|---|
| Authentication record — Google or Apple Sign-In (Firebase Auth) | Permanently deleted |
| Synced cards, saved offers, favourite merchants, and settings (Cloud Firestore) | Permanently deleted |
| Local app data (on-device SQLite database) | Cleared immediately by in-app deletion, or removed when the app is uninstalled |
| Analytics events (Firebase Analytics) | Deleted per Google's Firebase Analytics retention settings |

## What data is retained

No personal data is retained once the periods above have elapsed. Encrypted system backups may hold copies of deleted data for a short additional period before automated rotation removes them — see the [Privacy Policy]({{ '/privacy/' | relative_url }}) for details. Phronix does not store payment information, card numbers, or transaction history at any time.

---

*Last updated: 10 August 2026*
