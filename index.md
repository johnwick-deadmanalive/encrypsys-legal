# ENCRYPSYS — Privacy Policy

**Last updated:** 2026-04-24

This Privacy Policy explains how ENCRYPSYS ("the app", "we", "us") handles
your information when you use the Android application. By using ENCRYPSYS
you agree to the practices described below.

## 1. What ENCRYPSYS is

ENCRYPSYS is an end-to-end encrypted messaging application. Text messages
and voice messages are encrypted on your device before being sent and can
only be decrypted by the intended recipient. The operator of the service
cannot read the contents of your messages.

## 2. Information we collect

When you create an account and use the app, the following information is
stored on our backend (Google Firebase):

- **Email address** — used as your account identifier. Provided by you
  during sign-up.
- **Password** — never stored by the app. Handled by Firebase
  Authentication, which stores only a cryptographic hash.
- **Display name and username** — chosen by you during sign-up. Visible
  to your contacts.
- **Public encryption key** — generated on your device. Shared so others
  can encrypt messages to you. Your *private* key never leaves your
  device and is stored in the hardware-backed Android Keystore.
- **Push notification token (FCM token)** — used to deliver incoming
  message alerts to your device.
- **Contacts list** — the list of other ENCRYPSYS users you have added
  as contacts.
- **Encrypted messages** — message ciphertext and encrypted AES keys.
  We cannot decrypt these.
- **Typing indicators and read receipts** — ephemeral status flags.
- **Voice call signaling data** — session setup information
  (participants, call state). The audio of calls is transmitted
  peer-to-peer via WebRTC and is not stored on our servers.

We do **not** collect:

- Your address book or device contacts
- Your precise or approximate location
- Advertising or analytics identifiers
- Photos, videos, or files outside of what you send as messages

## 3. How your data is used

- **To provide the service** — delivering messages, routing calls,
  showing your contacts.
- **To authenticate you** — verifying your email and password at login.
- **To notify you** — sending push notifications when you receive
  messages or calls.

We do not sell, rent, or share your data with third parties for marketing
or advertising.

## 4. Third-party services

ENCRYPSYS uses the following services:

- **Google Firebase** (Authentication, Cloud Firestore, Cloud Messaging)
  — backend, account storage, encrypted message transport, push
  notifications. Firebase's privacy policy:
  https://firebase.google.com/support/privacy
- **coturn / TURN server** — used only during voice calls to relay
  encrypted audio packets when a direct peer-to-peer connection cannot
  be established. Call audio passes through the TURN server but remains
  encrypted by WebRTC's SRTP.

## 5. Encryption

- **Text and voice messages:** encrypted end-to-end using AES-256-GCM
  with per-message keys wrapped under each participant's RSA-2048-OAEP
  public key.
- **Private keys:** generated and stored only on your device in the
  Android Keystore. They are never transmitted.
- **Voice calls:** encrypted in transit using SRTP as provided by WebRTC.

## 6. Data retention and deletion

- Messages remain in our backend until deleted. You can delete a
  message you sent; the ciphertext is then overwritten and marked
  deleted in our database.
- If you delete your account, your `users` document, contacts list,
  and FCM token are removed. Historical encrypted messages in shared
  chats may remain on the recipient's device and in our database until
  the recipient deletes the chat.
- To request account deletion, contact us at the email below.

## 7. Children's privacy

ENCRYPSYS is not directed at children under 13. We do not knowingly
collect information from children under 13. If you believe a child
has provided us with information, contact us and we will delete it.

## 8. Security

We use industry-standard practices: all network traffic is over TLS,
message contents are end-to-end encrypted, and private keys are held
in hardware-backed secure storage where the device supports it.

No system is perfect. If we become aware of a breach that affects you,
we will notify affected users as required by applicable law.

## 9. Your rights

Depending on your jurisdiction (e.g. GDPR in the EU, CCPA in
California), you may have rights to access, correct, export, or delete
your personal data. To exercise these rights, contact us.

## 10. Changes to this policy

If we update this policy, the "Last updated" date at the top will
change. For material changes we will notify users in-app or by email.

## 11. Contact

For privacy questions or requests:

**Email:** rajanoumanmasood@gmail.com

---
