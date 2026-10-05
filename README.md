## COSMIC protocols (:construction: Work in Progress :construction:)
[![Continuous Integration](https://github.com/pop-os/cosmic-protocols/workflows/Continuous%20Integration/badge.svg)](https://github.com/pop-os/cosmic-protocols/actions?query=workflow%3A%22Continuous+Integration%22)
![LICENSE](https://img.shields.io/badge/LICENSE-GPL--3-brightgreen)
[![Docs](https://img.shields.io/badge/Docs-main-informational)](https://pop-os.github.io/cosmic-protocols/)

Additional wayland protocols and generated rust bindings used by the COSMIC desktop environment.

`kora_toplevel_identity::v1` binds [the toplevel identity protocol](unstable/kora-toplevel-identity-v1.xml).
It gives an application's own toplevel, or a live foreign handle, an atomic
identifier and authenticated process workspace. An empty workspace identifies
the machine plane; no workspace event means unknown. Visibility changes retain
the mapped lifetime's identity, while a true unmap closes it and a remap creates
a fresh identifier.
