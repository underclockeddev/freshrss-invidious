# FreshRSS - Invidious video extension

This FreshRSS extension allows you to directly watch Invidious videos from within subscribed channel feeds.

To use it, upload the ```xExtension-Invidious``` directory to the FreshRSS `./extensions` directory on your server and enable it on the extension panel in FreshRSS.

## Installation

The first step is to put the extension into your FreshRSS extension directory:
```
cd /var/www/FreshRSS/extensions/
git clone https://github.com/underclockeddev/freshrss-invidious
mv freshrss-invidious/xExtension-Invidious .
rm -rf freshrss-invidious/
```

Then switch to your browser https://www.my-freshrss-domain.com/i/?c=extension and activate it.

# Limitations

Currently only supports one hard-coded invidious instance, inv.tux.pizza. I intend to make this configurable in the future.

# Features

- Embeds Invidious videos directly in FreshRSS, instead of linking to the Invidious page
- Simplifies the subscription to channel URLs by automatically detecting the channels feed URL

You can simply add Invidious video subscriptions by pasting URLs like:
- `https://inv.tux.pizza/channel/UCddn8dUxYdgJz3Qr5mjADtA` 

# Contributions

- This extension is based very heavily on the work of @kevinpapst https://github.com/kevinpapst/freshrss-youtube

## About FreshRSS

[FreshRSS](https://freshrss.org/) is a great self-hosted RSS Reader written in PHP, which is can also be found here at [GitHub](https://github.com/FreshRSS/FreshRSS).

More extensions can be found at [FreshRSS/Extensions](https://github.com/FreshRSS/Extensions).
