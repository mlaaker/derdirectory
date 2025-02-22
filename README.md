# DER Directory
## _A [Homebrew-style](https://brew.sh/) catalog & API for connected home/business energy-making/saving devices & the virtual power plants with which they can connect_
Programmatically-accessible catalog of the various interconnection and management opportunities as well as security characteristics of Distributed Energy Resources (DER) devices (whether for consumer or commercial usage) to outline which products may or may not work with your smart home network (Hubs) and/or [Virtual Power Plant (VPP)](https://rmi.org/clean-energy-101-virtual-power-plants/) provider(s). By exposing this catalog in this manner, anyone can create/edit device, hub, and VPP 'recipes' to ensure the community has the latest information on these devices' capabilities and connections. 



### Uses
Imagine if your home-/business-level management layer (a Hub, like your Alexa, Google Home, or Home Assistant), which already knows all/most of the devices in your home, could 
* identify which of your devices in your home/business are **eligible for enrollment in an VPP** to _earn you money_ (whether by adjusting your temperature or reducing power during peak system loads)
* know _which_ of your existing devices are enrolled in which VPP programs and **communicate real-time credits/payments**
* identity **what _new_ devices might best work with and support your existing** home/business infrastructure to add more VPP-capable connections. 


### API
**Not yet available.** Once a reasonable corpus of devices, hubs, and VPPs are documented, an API will be made available to:
* **Product** - _(input: product-name)_ return all details for a given product
* **VPP support** - _(input: product-name, vpp-name)_ return an array of true/false for each market for whether the VPP supports this device type
* **Hub compatibility** - _(input: product-name, hub-name)_ return true/false for whether the hub supports this device type


### Reference

See examples:
* [Kasa Smart Wi-Fi Plug Slim with Energy Monitoring KP125M](https://github.com/mlaaker/derdirectory/blob/main/devices/outlets/tp-link-kasa-kp125m.json) (See [all devices…](https://github.com/mlaaker/derdirectory/tree/main/devices))
* [Renew Home OhmConnect](https://github.com/mlaaker/derdirectory/blob/main/vpp/renew-home-ohmconnect.json) (See [all VPPs…](https://github.com/mlaaker/derdirectory/tree/main/vpp))
* [Home Assistant Yellow](https://github.com/mlaaker/derdirectory/blob/main/devices/hubs/home-assistant-yellow.json) (See [all Hubs…](https://github.com/mlaaker/derdirectory/tree/main/devices/hubs))

