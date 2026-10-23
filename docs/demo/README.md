# Editor capture

Captured on 2026-10-23 from source revision
`86269a6a1ae633355f55da41563e096145f2b5b4`.

The app ran with Node.js, Bun-installed locked dependencies and Next.js 14.2.35
on Linux. Authentication used disposable local values. MongoDB 8.0 ran in an
isolated Docker container published only on loopback. No existing deployment,
real project database or model API was used.

The browser signed in, reloaded the editor to create an authenticated project,
opened Design → Content and changed the headline, supporting text, author and
topic. `editor.png` captures the actual UI. Clicking Export PNG produced
`poster.png`, a 222443-byte file. After allowing the save delay, a page reload
retained the edited headline. The browser reported no page errors.

The capture demonstrates manual editing, local saving, reload and PNG export.
It does not test generation, production deployment, mobile layout or every
preset. The initial unauthenticated project-create request required a reload
following sign-in.
