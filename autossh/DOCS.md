# barisozdag's Personal Home Assistant Add-ons: Autossh

Simple autossh addon. The addon creates a ssh keypair, and uses it
to connect to to the given host. The public key can be found in the
log after the first startup.

Remember to set `GatewayPorts clientspecified` in sshd-config if you
would like to open ports on other interfaces than localhost.

**IMPORTANT**: If you set `GatewayPorts yes`, all forwarded ports will
listen on all interfaces, `0.0.0.0`. `GatewayPorts clientspecified`
is preferable.

## Installation

The installation of this add-on is pretty straightforward and not different in
comparison to installing any other Home Assistant add-on.

1. Click the Home Assistant My button below to open the add-on on your Home
   Assistant instance.

   [![Open this add-on in your Home Assistant instance.][addon-badge]][addon]

1. Save the add-on configuration.
1. Start the "Autossh" add-on.
1. Check the logs of the "Autossh" to see if everything went well.
1. Copy the public key to the remote server.

## Configuration

**Note**: _Remember to restart the add-on when the configuration is changed._

Example add-on configuration:

```yaml
hostname: domain.server.com
ssh_port: 22
username: autossh
remote_forwarding:
  - 127.0.0.1:8123:172.17.0.1:8123
local_forwarding:
  - ""
other_ssh_options: "-v"
monitor_port: "0"
gatetime: "30"
```

**Note**: _This is just an example, don't copy and paste it! Create your own!_

## Changelog & Releases

This repository keeps a change log using [GitHub's releases][releases]
functionality.

Releases are based on [Semantic Versioning][semver], and use the format
of `MAJOR.MINOR.PATCH`. In a nutshell, the version will be incremented
based on the following:

- `MAJOR`: Incompatible or major changes.
- `MINOR`: Backwards-compatible new features and enhancements.
- `PATCH`: Backwards-compatible bugfixes and package updates.

## Support

Got questions?

You could [open an issue here][issue] GitHub.

## Authors & contributors

The original setup of this repository is by [Odin Udegal][odinuge].
This repository is a copy of [Odin Ugedal's Hassio Addons][odin_hassio_addons]
without the `frpc` addon.

For a full list of all authors and contributors,
check [the contributor's page][contributors].

## License

MIT License

Copyright (c) 2017-2020 Odin Ugedal

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

[addon-badge]: https://my.home-assistant.io/badges/supervisor_addon.svg
[addon]: https://my.home-assistant.io/redirect/supervisor_addon/?addon=bb761233_autossh&repository_url=https%3A%2F%2Fgithub.com%2Fbarisozdag%2Fhaddons-repo
[contributors]: https://github.com/barisozdag/addon-autossh/graphs/contributors
[odinuge]: https://github.com/odinuge
[odin_hassio_addons]: https://github.com/odinuge/hassio-addons
[issue]: https://github.com/barisozdag/addon-autossh/issues
[releases]: https://github.com/barisozdag/addon-autossh/releases
[semver]: https://semver.org/spec/v2.0.0.html
