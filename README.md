# DER Directory
## _A [Homebrew-style](https://brew.sh/) B2B(2C) catalog & API of connected home/business energy-making/saving devices & the virtual power plants with which they can connect_

**Problem statement:** Understanding whether any of your existing home or business' devices can connect with money-returning [Virtual Power Plant (VPP)](https://rmi.org/clean-energy-101-virtual-power-plants/) services, much less which _potential_ devices could work in your existing setup _and_ earn you money is a maddeningly complex, regionally different, byzantine process that is not conducive to _expediting humanity’s move to clean all-electric power & a grid that can support that sizable shift._

DER Directory is a **programmatically-accessible catalo**g of the various interconnection and management opportunities as well as security characteristics of Distributed Energy Resources (DER) devices (whether for consumer or commercial usage) to outline which products may or may not work with your smart home network (Hubs) and/or VPP provider(s). By exposing this catalog in this manner, anyone can create/edit device, hub, and VPP 'recipes' to ensure the community has the latest information on these devices' capabilities and connections. 



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


### Examples

The following are examples of the community-editable configuration files that would provide the data to the API for this project:
* [Kasa Smart Wi-Fi Plug Slim with Energy Monitoring KP125M](https://github.com/mlaaker/derdirectory/blob/main/devices/outlets/tp-link-kasa-kp125m.json) _(See [all devices…](https://github.com/mlaaker/derdirectory/tree/main/devices))_
* [Renew Home OhmConnect](https://github.com/mlaaker/derdirectory/blob/main/vpp/renew-home-ohmconnect.json) _(See [all VPPs…](https://github.com/mlaaker/derdirectory/tree/main/vpp))_
* [Home Assistant Yellow](https://github.com/mlaaker/derdirectory/blob/main/devices/hubs/home-assistant-yellow.json) _(See [all Hubs…](https://github.com/mlaaker/derdirectory/tree/main/devices/hubs))_



### FAQs

#### Who has to participate for this to have value?
Value from this project can be seen in a number of ways (see FAQs below), but for any value to be accrued, at least two things need to happen:

1. **Contributions of data**: ideally, OEM manufacturers would begin providing the data as the technical owners who know the most details about their products. However, the Homebrew project has shown that individuals, customers, home/small businesses owners willingly provide far more onerous details and solutions On their own as they improve their home management layer (Hub) experience. Contributions could easily be made by anyone with a GitHub account and a browser.
2. **Exposure of data**: At present, the biggest point of leverage for the use of the data would be in the home management layer (hubs) as they would provide (with a single integration) home/business owners (who already have these Hub devices installed) visibility to the VPP enrollment, device compliance, and additional device compatibility opportunities. 



#### What does an device manufacturer (OEM) get?

By contributing up-to-date information about their devices, OEMs can increase the sales of their devices (and the kickbacks VPPs many times offer them from successful enrollments) by increasing the chances of home/business owners discovering their products are available, compatible with their systems, and verified to work with a local VPP. 
​

#### What does a VPP get? 

By enabling Hubs to expose awareness of available VPPs to customers, AND attestation of which devices they currently own which can be leveraged by the VPP, AND then surface which additional OEM devices could further increase their earnings while working with the customer’s system 



#### What does a utility get?

To meet the dramatic increase in power generation needs in a world where utilities physically cannot build the infrastructure fast enough, increased capacity in and leverage of VPPs offer one (of many needed) way to meet their region’s power needs without additional instructor buildout. 



#### What does a homeowner/business owner get?

Home/business owners and renters can discover ways to earn money through their smart home investments (helpful to this projects’s ultimate goal), AND simplify understanding of what additional devices would work with the system they already have (beyond the purpose of this project’s initial goals), AND have a better understanding of their home network security(beyond the purpose of this project’s initial goals).



#### Is this a new communication channel VPPs, OEMs, or Hubs need to adopt?

No. The communication protocols VPPs use to communicate with customers’ OEM devices can remain the same. The VPP never has to talk to the customer’s Hub, although there are plenty of customer experience improvements that would come from that shift (namely; customer’s data privacy, network security, and management experience fatigue). 

​In a future state where Hubs have better awareness of their connected OEM devices AND the VPP(s) being leveraged, there are strong customer incentives to have VPPs talk to the Hubs (rather than to the OEM devices) to give customers a single “pane of glass” to manage their home/business (rather than continue the proliferation of dozens of OEM mgmt. apps on top of the Hub and VPP