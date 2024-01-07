# barisozdag's Personal Home Assistant Add-ons: Cloud Commander

[Cloud Commander][cloudcmd] is a file manager for the web. It includes a
command-line console and a text editor. Cloud Commander helps you manage your
server and work with files, directories and programs in a web browser from
any computer, mobile or tablet.

## Installation

The installation of this add-on is pretty straightforward and not different in
comparison to installing any other Home Assistant add-on.

1. [![Add repository to your Home Assitant instance.][repository-badge]][repository]
1. Click the Home Assistant My button below to open the add-on on your Home
   Assistant instance.

   [![Open this add-on in your Home Assistant instance.][addon-badge]][addon]

1. Save the add-on configuration.
1. Start the "CloudCMD" add-on.
1. Check the logs of the "CloudCMD" to see if everything went well.
1. Login to the web interface.

## Web-UI

Web-UI can be found at `<your-ip>:8000`.

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

The original setup of this repository is by [Barış Özdağ][barisozdag].

For a full list of all authors and contributors,
check [the contributor's page][contributors].

## License

MIT License

Copyright (c) 2023 Barış Özdağ

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
[addon]: https://my.home-assistant.io/redirect/supervisor_addon/?addon=bb761233_cloudcmd
[contributors]: https://github.com/barisozdag/addon-cloudcmd/graphs/contributors
[barisozdag]: https://github.com/barisozdag
[issue]: https://github.com/barisozdag/addon-cloudcmd/issues
[cloudcmd]: https://github.com/coderaiser/cloudcmd
[releases]: https://github.com/barisozdag/addon-cloudcmd/releases
[repository-badge]: https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg
[repository]: https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2Fbarisozdag%2Fhaddons-repo
[semver]: https://semver.org/spec/v2.0.0.html