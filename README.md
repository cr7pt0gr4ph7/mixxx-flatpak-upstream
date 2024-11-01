# Flatpak manifest for `io.github.cr7pt0gr4ph7.Mixxx.Upstream`
## What's this?
This is a custom Flatpak build of [Mixxx](https://mixxx.org/) based on the `main`
branch of [mixxxdj/mixxx](https://github.com/mixxxdj/mixxx/tree/main),
i.e. the bleeding edge of Mixxx development.

See [cr7pt0gr4ph7/mixxx-flatpak](https://github.com/cr7pt0gr4ph7/mixxx-flatpak)
for an alternative version that also includes my custom patches.

The ID of the Flatpak has been modified to be `io.github.cr7pt0gr4ph7.Mixxx.Upstream`
instead of `org.mixxx.Mixxx`, so it ispossible to install it in parallel
to an already existing "official" Mixxx installation.

I run an atomic [Fedora Silverblue](https://fedoraproject.org/atomic-desktops/silverblue/)
desktop based on [Bluefin](https://projectbluefin.io/) where almost all apps are installed
via [Flatpak](https://flatpak.org/) only, so this is the way I provide myself with
a clean alpha build of the changes I am trying to get merged into the upstream project.
Due to the bleeding-edge nature of the code, it might crash, have bugs, corrupt the database,
or just not work as expected, and is therefore probably unsuitable for critical production use, YMMV.

## How do I use it?

The flatpak images are published to a flatpak repository hosted via GitHub pages.
You can add the repository and install the flatpak image using the following commands:

```bash
sudo flatpak remote-add --if-not-exists mixxx-flatpak https://cr7pt0gr4ph7.github.io/mixxx-flatpak-upstream/default.flatpakrepo
sudo flatpak install io.github.cr7pt0gr4ph7.Mixxx.Upstream
```

As noted above, this is a bleeding edge build used for testing purposes, and no guarantees are given regarding the stability or bugginess. Use at your own risk!

## Acknowledgements

- [The Mixxx Team](https://github.com/mixxxdj/mixxx)
- [andyholmes/flatter](https://github.com/andyholmes/flatter)
