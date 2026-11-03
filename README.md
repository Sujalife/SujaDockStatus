# Suja Dock Status

Standalone frontend for docks 16–19, sharing accounts, roles, messages, and themes with [Suja Life Tools](https://github.com/Sujalife/SujaLifeTools).

**Firebase web app configuration is included; live backend activation remains pending.** Open Explore demo for explicitly labeled browser-only sample data.

The authoritative shared backend, rules, setup instructions, and tests are in SujaLifeTools. This export never deploys a separate backend.

Set Settings → Pages → Source → GitHub Actions to publish the frontend. The workflow verifies assets and JavaScript syntax. Deployment does not activate Firebase.

The supplied public Firebase config is included in dist/shared/config.js. Authentication, backend functions, rules, and the Master account still require activation in the authoritative hub project. Both repository paths on sujalife.github.io share Firebase authentication persistence.

Built with native-generated art and the existing Suja light/dark palette.
