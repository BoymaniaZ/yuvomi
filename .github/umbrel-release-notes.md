<!-- version: 2.81.2 -->
This is a security release, and it changes nothing about how Yuvomi looks or works day to day. It completes the Web Push fix from 2.81.1: a specially crafted push address could still get past the new check and make the server connect into your own network. Push addresses are now checked the same way the push library reads them.

Push notifications to phones and browsers keep working as before. A stored push subscription with an unusual address is removed on its next delivery, like an expired one.

Nothing changes in the database with this update, so it is a plain container swap with no migration to wait for.

Full release notes are available at https://github.com/ulsklyc/yuvomi/releases/tag/v2.81.2
