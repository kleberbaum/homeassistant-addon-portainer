# Home Assistant Custom Add-on: Portainer

![Warning][warning_stripe]

> This is a **fork** of the deprecated [community add-on][community_addon]!
>
> This makes it available again.

![Warning][warning_stripe]

Portainer is an open-source lightweight management UI which allows you to
easily manage a Docker host(s) or Docker swarm clusters.

It has never been so easy to manage Docker. Portainer provides a detailed
overview of Docker and allows you to manage containers, images, networks and
volumes.

## Installation

To install this add-on, you'll first need to go to your profile and turn on
"Advanced Mode", once that is done go back to Home Assistant add-ons and search
for "Portainer" and install it as you would any other add-on.

To be able to use this add-on, you'll need to disable protection mode on this
add-on. Without it, the add-on is unable to access Docker.

1. Navigate in your Home Assistant frontend to **Settings** -> **Add-ons** ->
   **Add-on Store**.
1. In the **...** menu at the top right corner click **Repositories**, add
   `https://github.com/kleberbaum/homeassistant-addon-portainer` as repository.
1. Find the "Portainer" add-on and click it. If it doesn't show up, wait until
   HA refreshes the information about the add-on, or click **Check for updates**
   in the **...** menu at the top right corner.
1. Click on the "INSTALL" button.

## How to use

1. Under the Info tab set the "Protection mode" switch to off.
1. Start the add-on.
1. Check the add-on log output to see the result.

## Add-on Configuration

```yaml
agent_secret: password
```

### Option: `agent_secret`

An option to set a shared agent secret. Must also be set in the remote agent
as an Environment variable.

## Support

Got questions?

You have several options to get them answered:

- The [Home Assistant Discord chat server][discord].
- The Home Assistant [Community Forum][forum].
- Join the [Reddit subreddit][reddit] in [/r/homeassistant][reddit]

You could also [open an issue here][issue] on GitHub.

## Authors & contributors

The original setup of this repository is by [Franck Nijhof][frenck].

For a full list of all authors and contributors,
check [the contributor's page][contributors].

## License

MIT License

Copyright (c) 2018-2021 Franck Nijhof

Copyright (c) 2022-2023 Laszlo Magyar

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

[contributors]: https://github.com/kleberbaum/homeassistant-addon-portainer/graphs/contributors
[discord-ha]: https://discord.gg/c5DvZ4e
[discord]: https://discord.me/hassioaddons
[forum]: https://community.home-assistant.io/t/home-assistant-community-add-on-portainer/68836?u=frenck
[frenck]: https://github.com/frenck
[issue]: https://github.com/kleberbaum/homeassistant-addon-portainer/issues
[reddit]: https://reddit.com/r/homeassistant
[semver]: http://semver.org/spec/v2.0.0.html
[warning_stripe]: https://github.com/kleberbaum/homeassistant-addon-portainer/raw/main/images/warning_stripe_wide.png
[community_addon]: https://github.com/hassio-addons/addon-portainer
