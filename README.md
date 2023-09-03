# dns-base
[![ci-main](https://github.com/joris-me/dns-base/actions/workflows/ci-main.yml/badge.svg)](https://github.com/joris-me/dns-base/actions/workflows/ci-main.yml)
[![GitHub tag (with filter)](https://img.shields.io/github/v/tag/joris-me/dns-base?filter=v*&label=release)](https://github.com/joris-me/dns-base/pkgs/container/dns-base)

This is a [CoreDNS](https://coredns.io/) image with additional plugins enabled:
- [alternate](https://coredns.io/explugins/alternate/)
- [records](https://coredns.io/explugins/alternate/)

It is used by downstream projects in the [joris.me ecosystem](https://github.com/joris-me), such as [dns-mock-tailscale](https://github.com/joris-me/dns-mock-tailscale) and [stack-coredns](https://github.com/joris-me/stack-coredns).

The produced image comes with a rudimentary [Corefile](/dns-base/Corefile) configured with the [whoami](https://coredns.io/plugins/whoami/) plugin.

For additional info about CoreDNS, see the [CoreDNS README](coredns/README.md).

## Configuration
Mount your `Corefile` at `/Corefile` in the container.
