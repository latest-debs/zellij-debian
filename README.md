![zellij for Debian](.github/readme-header.png)

# zellij for Debian

[zellij-org/zellij](https://github.com/zellij-org/zellij) — A terminal workspace and multiplexer with built-in layouts, session persistence, and a plugin system. —
packaged for Debian as part of [latest-debs](https://github.com/latest-debs).

Want your own project packaged and maintained this way? See the
[latest-debs packaging service](https://github.com/latest-debs/apt-repo/blob/main/SERVICE.md).

## Install

Via the latest-debs apt repository:

```sh
sudo extrepo enable latest-debs
sudo apt update
sudo apt install zellij
```

Or download a `.deb` from the [Releases](https://github.com/latest-debs/zellij-debian/releases) page:

```sh
sudo dpkg -i zellij_*.deb
```

## Supported distributions & architectures

- Debian Bookworm (12), Trixie (13), Forky (14/testing), Sid (unstable)
- amd64, arm64, armhf, i386, ppc64el, riscv64, s390x — whichever
  architectures zellij-org/zellij actually publishes a Linux binary for

## Disclaimer

Unofficial, volunteer-run packaging — **best-effort, no SLA**.

- **Update cadence:** publishing a release normally triggers an immediate
  apt-repo rebuild via webhook; the ~6h scheduled run is the fallback. GitHub
  outages, a missing trigger token, rate limits, or upstream archive changes
  can delay or skip an update; there is no freshness guarantee.
- **Draft releases:** every build is published as a *draft* that a maintainer
  reviews before promoting, so a new version can lag its build.

For issues with zellij itself, see
[zellij-org/zellij](https://github.com/zellij-org/zellij).
