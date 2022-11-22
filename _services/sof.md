---
title: "SOF"
date: 2018-11-18T12:33:46+10:00
weight: 1
tags: [Mermaid]
mermaid: true
---

Portcall data is preloaded from VMS. Automated flow and real time registration prevents errors and ensures good data accuracy and quality. **Real time connection and digital signing** process reduces the need for manual communication between agents, operations and vessels. The application has offline capabilities and supports bad connections while in port

![SOF Services](/images/stock/theship-sof-front.jpg)

# Statement of facts data collection
## Getting started

For starting testing the digital statement of facts service we can get you **up and running in just a day**. The fine tuning of company information and settings together with your templates requires that you set aside a week, and together we'll make your statement of facts accordingly to your wishes and you'll see data coming in from portcall number one.

### How to obtain a company subscription
Your company needs to registered in our master data and we'll get you up and running in no time. **Send us a mail with your logos and these identifying data[^1]**

 1. Company name
 2. Street address (HQ)
 3. Zip(HQ)
 4. City(HQ)
 5. Country(HQ)
 6. Email (account responsible)
 7. Phone (account responsible)
Your account will be up and running in no time.

[^1]: No customer identifying data will be shared

### Update company templates
When you are generating statement of facts, voyage reports, demurrage claim or other activities that demands the generation of a document you want them to look as professional and clean as possible, but with all required data every time. You will start out with our easy to understand templates to make them look as good as possible. 

### Word and html templating
We use word and html as our baseline templates for document generation. We know that making a document look good every time is important. Both Word and Html-templates are probably not something you do every day. We are experts in this and got you covered. Just send us the ones you are using today and we'll make them into templates - we'll maybe even improve them a little, but only if necessary.  

### Create Statement of facts data collection flow
In our experience, it differs from company to company and segment to segment what data are named and what they are used for. And in the agile flow that secures the input quality during collection makes this possible.
You can collect the data you need and even the data you need for other analyses. We got some initial templates for **tankers**, **dry bulk**, **container** or **RO-RO** vessels that will get you started. It can be a daunting experience the first time you start editing these flows, but as a part of our onboarding we help you get you first data collection flow drawn up.

![](/images/stock/ship-flow-full.jpg)



### Create vessels, partners and contact persons
> NOTE: If you choose integrate your VMS or other line of business systems with The Ship all vessels,  partners, voyages, portcalls and cargos are synced with your application ( [jump](#integration) to read about integration )

If you are not integrated with the ship services you need to add your vessels, partners, contacts to your configuration, so that you can start using the sof collector application on board vessels.
Our port library and commodities lists are growing each day, but if you are missing a port or commodity you need to add this.

### Create app users
Your almost there. Beside the company users you must create App users or Agent users that will do the actual data collection and statement of fact document generation during portcalls.
> App user. One or more personnel using the application onboard a vessel
> Agent user. An agent responsible for servicing you at a specific port

![](/images/stock/app-agent-users.jpg)

### You are ready to start using our services

## Create voyages
> NOTE: If you choose integrate your VMS or other line of business systems with The Ship all vessels,  partners, voyages, portcalls and cargos are synced with your application ( [jump](#integration) to read about integration )

### Create voyage details
### Create Port call schedule
### Create Cargo details

<div id="integration"></div>
## Integration makes day to day operations smooth sailing
Coming...

### Synchronization master data
<div class="mermaid">
sequenceDiagram
TheShip -->> VMS: Hello VMS  , do you have updates for me?
VMS-->>TheShip: Yes, here
</div>

### Synchronization messages
<div class="mermaid">
sequenceDiagram
Sof -->> MessageHub: Here are my changes
MessageHub -->>CustomerQueue: Incoming messages
MessageHub -->>TheShipCoreQueue: Incoming messages
</div>
