=======
Changes
=======


1.3.1
-----

* Allow Pyramid 2. The cap was in pyproject.toml but never reached PyPI until
  1.3: 1.2 published without one and has been running against Pyramid 2 ever
  since, while 1.3 published the cap and so pulled dependants back down to
  Pyramid 1. Upgrade straight to this release; 1.3 is best avoided.
  [zupo]


1.3
---

* Add `pyramid_cloudflare_access.bypass_hosts`, for naming the hostnames that
  skip the Cloudflare Access check, such as Fly.io review apps. Defaults to
  `herokuapp.com`, which is what was skipped before.
  [zupo]

* Match bypassed hostnames by whole domain labels rather than by substring, so
  that a lookalike such as `herokuapp.com.attacker.example` is verified like
  any other hostname.
  [zupo]


0.1
---

* Initial release.
  [dz0ny, zupo]

