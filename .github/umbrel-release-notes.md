<!-- version: 2.81.1 -->
This is a security release, and it changes nothing about how Yuvomi looks or works day to day. Two issues are fixed: the image now runs on a Node.js version that closes a flaw in its built-in Brotli decoder, which a crafted compressed stream could use to crash the server or, in the worst case, run code; and Web Push notifications can no longer be pointed at addresses inside your own network, and a push service that does not answer now gives up after 10 seconds instead of holding up reminders.

Push notifications to phones and browsers keep working as before. A stored push subscription with an internal address is removed on its next delivery, like an expired one.

Nothing changes in the database with this update, so it is a plain container swap with no migration to wait for.

Full release notes are available at https://github.com/ulsklyc/yuvomi/releases/tag/v2.81.1
