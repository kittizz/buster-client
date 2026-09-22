<p align="center"><img width="128" height="128" src="https://i.imgur.com/uVpmR8l.png"></p>
<h1 align="center">Buster Client</h1>

<p align="center">
  </br></br>
  <a href="https://github.com/kittizz/buster-client/releases/latest">
    <img src="https://i.imgur.com/8y9ep17.png" alt="Windows"></a>
  <a href="https://github.com/kittizz/buster-client/releases/latest">
    <img src="https://i.imgur.com/ewvx5hO.png" alt="Linux"></a>
  <a href="https://github.com/kittizz/buster-client/releases/latest">
    <img src="https://i.imgur.com/eTc9xGf.png" alt="macOS"></a>
  </br></br>
</p>

## About This Fork

This is an unofficial community fork of
[dessant/buster-client](https://github.com/dessant/buster-client), whose
pinned dependencies had gone stale since 2020. Changes made here:

- Added native Apple Silicon (macOS arm64) and Windows arm64 builds —
  neither was buildable upstream, since the pinned `robotgo`/`gopsutil`
  versions predated Apple Silicon, modern macOS SDKs, and `windows/arm64`.
- Modernized dependencies (`robotgo` v1.0.2, `gopsutil` v4,
  `golang.org/x/sys`) so the client builds on current toolchains for all
  five supported OS/arch combinations, while keeping the native-messaging
  protocol version (`0.3.0`) unchanged for compatibility with the
  currently published Buster extension.
- Added Brave browser support (native-messaging manifest paths on Linux
  and macOS).
- Added [`mise.toml`](mise.toml) pinning `go`, `node`, `yarn`, and `zig`
  (used to cross-compile the Windows builds) for reproducible local
  toolchain setup.

Releases are published at
[kittizz/buster-client/releases](https://github.com/kittizz/buster-client/releases).
For the original, upstream project, see
[dessant/buster-client](https://github.com/dessant/buster-client).

## Supporting the Project

The continued development of Buster is made possible
thanks to the support of awesome backers. If you'd like to join them,
please consider contributing with
[Patreon](https://armin.dev/go/patreon?pr=buster-client&src=repo),
[PayPal](https://armin.dev/go/paypal?pr=buster-client&src=repo) or
[Bitcoin](https://armin.dev/go/bitcoin?pr=buster-client&src=repo).

## Description

Buster Client is a native app used by the [Buster](https://github.com/dessant/buster#readme)
extension to simulate user interactions.

## Installation

Download the [latest release](https://github.com/kittizz/buster-client/releases/latest)
of the client app for your OS and architecture (macOS arm64/amd64, Linux
amd64, or Windows arm64/amd64) and follow the
[installation guide](https://github.com/dessant/buster/wiki/Installing-the-client-app)
for your operating system.

## Issues

Open issues about the browser extension itself on the
[main repository](https://github.com/dessant/buster/issues). Issues
specific to this fork's builds or toolchain can be opened on
[this repository](https://github.com/kittizz/buster-client/issues).

## License

Copyright (c) 2019-2022 Armin Sebastian

This software is released under the terms of the GNU General Public License v3.0.
See the [LICENSE](LICENSE) file for further information.

The operating system icons are provided by [Icons8](https://icons8.com).
