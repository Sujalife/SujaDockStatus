# Suja Dock Status

Standalone frontend for docks 16–19, sharing accounts, roles, messages, and themes with [Suja Life Tools](https://github.com/Sujalife/SujaLifeTools).

This version uses **direct Firebase Authentication and Realtime Database access protected by rules**. Core operation requires no Cloud Functions deployment or Blaze upgrade. Firebase's service limits still apply.

The supplied public Firebase configuration is included. **Live activation still requires the matching version 2 rules and the owner UID at toolsV2/config/masterUid.** The authoritative rules, setup instructions, and tests are maintained in [SujaLifeTools](https://github.com/Sujalife/SujaLifeTools/blob/main/SETUP.md). This export does not deploy a separate backend or maintain a second rules copy.

Use Create account to make a pending identity and copy its UID. Only a Firebase project administrator can pin Master in the Console; the first visitor never becomes Master automatically. The Master approves other accounts and assigns roles. Both repository paths on sujalife.github.io share Firebase authentication persistence.

The dock board and hub support icon/card and list views. The interface shows the last 72 hours of history and messages; authorized open apps clean up expired entries while active. Physical deletion is not guaranteed while every browser is closed, and current dock status is retained.

Choose Explore demo for labeled browser-only sample data. Demo updates never write to Firebase.

Set Settings → Pages → Source → GitHub Actions to publish the frontend. Pages publication does not publish Firebase rules.

Shared source changes belong in SujaLifeTools and should be exported to this repository together. Native-generated artwork and the existing Suja light/dark palette are preserved.
