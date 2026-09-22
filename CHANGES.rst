=======
Changes
=======


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

