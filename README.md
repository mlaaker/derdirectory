# DER Directory
Programmatically-accessible catalog of the various interconnection and management opportunities as well as security characteristics of Distributed Energy Resources (DER) devices (whether for consumer or commercial usage) to outline which products may or may not work with your smart home network (Hubs) and/or VPP provider(s).

See examples:
* [Kasa Smart Wi-Fi Plug Slim with Energy Monitoring KP125M](https://github.com/mlaaker/derdirectory/blob/main/devices/outlets/tp-link-kasa-kp125m.json) (See [all devices…](https://github.com/mlaaker/derdirectory/tree/main/devices))
* [Renew Home OhmConnect](https://github.com/mlaaker/derdirectory/blob/main/vpp/renew-home-ohmconnect.json) (See [all VPPs…](https://github.com/mlaaker/derdirectory/tree/main/vpp))
* [Home Assistant Yellow](https://github.com/mlaaker/derdirectory/blob/main/devices/hubs/home-assistant-yellow.json) (See [all Hubs…](https://github.com/mlaaker/derdirectory/tree/main/devices/hubs))


## API
Once a reasonable corpus of devices, hubs, and VPPs are documented, an API will be made available to:
* **Product** - _(input: product-name)_ return all details for a given product
* **VPP support** - _(input: product-name, vpp-name)_ return an array of true/false for each market for whether the VPP supports this device type
* **Hub compatibility** - _(input: product-name, hub-name)_ return true/false for whether the hub supports this device type

