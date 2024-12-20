[![NPM](https://img.shields.io/npm/v/@hernas/homebridge-salus-sq610)](https://npmjs.org/package/@hernas/homebridge-salus-sq610)
[![verified-by-homebridge](https://badgen.net/badge/homebridge/verified/purple)](https://github.com/homebridge/homebridge/wiki/Verified-Plugins)

# homebridge-salus-sq610
Salus plugin for [HomeBridge](https://github.com/nfarina/homebridge) using a the Salus UG600 universal gateway on the local network to expose Salus Thermostats to Apple's HomeKit.

**Supported devices:**
* SQ610
* SQ610RF
* VS20WRF
* VS10WRF

![HomeKit Screenshot](.github/statics/homekit-1.png)

## Things to know
* Plugin implements all modes of heating, but let's the thermostate decide if it is in cooling or heating mode. (for example by shorting S1 & S2 pins on the board)

## Getting started

### Sample configuration
```
{
  "platform": "SalusSQ610HomebridgePlugin",
  "ip_address": "<UGW ip address like 192.168.0.100>",
  "eu_id": "<Either 0000000000000000 or provide real euid from the bottom side of UGW>"
}
```

### Legal
* Licensed under [MIT](LICENSE)
* This is not an official plug-in and is not affiliated with Salus in any way
