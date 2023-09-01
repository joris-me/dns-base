# dns-base
This is a [CoreDNS](https://coredns.io/) image with additional plugins enabled:
- [alternate](https://coredns.io/explugins/alternate/)
- [records](https://coredns.io/explugins/alternate/)

It is used by downstream projects in the [joris.me ecosystem](https://github.com/joris-me), such as [dns-mock-tailscale](https://github.com/joris-me/dns-mock-tailscale) and [stack-coredns](https://github.com/joris-me/stack-coredns).

The produced image comes with a rudimentary [Corefile](/dns-base/Corefile) configured with the [whoami](https://coredns.io/plugins/whoami/) plugin.

For additional info about CoreDNS, see the [CoreDNS README](coredns/README.md).

## Configuration
```bash
docker pull 

```
Mount your `Corefile` at `/etc/coredns/Corefile` in the container.