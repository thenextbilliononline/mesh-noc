# mesh-noc
This will be a stand-up mesh network operations center for new mesh locals to get up and go. Ideally the server infrastructre would be relatively independent (i.e. Wekan/BGP wouldn't have to be same device, but could be).

Mesh Networking has arisen as a viable alternative when communities are otherwise disconnected. Mesh networks have been used to provide [emergency access in NYC](redhook wifi), connect otherwise unconnected communities (Altermundi), and provide basic internet access to wide populations both urban and rural (Freifunk, Guifi, NYC Mesh).  These distributed networks provide the kinds of network topologies that are resistant to network outages, quality degradation, and moving base stations. In that way, they are particularly suited to emergency situations and deployment by non-technical people.

The mesh networking movement started with a linux distribution for routers called Openwrt which was installed mainly on commercially available small-office/home-network routers with minimal specifications. Other, commercially available products like Ubiquiti Wireless Internet Service Provider products and other long-range setups have been adopted by the community. However, both types of device has shown their drawbacks. Small-office/home-network routers have limited range and tend to broadcast equally in all directions, indifferent to whether or not that benefits the end user. Point to point or point to multi-point antennas (like Ubiquiti products) require extensive site surveys, link planning, and a considerable up-front investment. Often these are only worthwhile if a user can guarantee that they will not move location for years. The beauty of  the mesh network topology is that it isn't reliant on a particular network configuration. It judges link quality autonomously and chooses the best route for its users. Libremesh, a particular implementation of this mesh networking technology is used by communities across the world from Freifunk in Germany, Guifi.net in Spain and Altermundi in Argentina. Collectively, they have deployed 50,000 access points in a conglomeration of municipal, community, and individual interests to create interoperable and open source networks.

## Problem

After many years of using commercially available hardware, Altermundi, in conjunction with many other groups, started developing the ultimate mesh hardware. These have been in testing since last year as prototypes and the results are very promising. The radios are capable of 150Mbps connections covering a radius of 200 meters. In NYC, that could provide internet access to an entire building for $150. In Argentina, a single unit is capable of providing connectivity to  an entire village. However, the open source software is missing some components that are widely available in commercial and proprietary implementations. It is very difficult to start a new mesh from scratch. Ad-hoc networks are not very good at documentation and each locale builds components in parallel. Additionally,the BGP, organizational, and web infrastructure if very technical and hard to maintain. Finally, the open-source software stack lacks any practical way for communities to monitor network quality and distribute resources fairly. Thus far, communities have relied on good neighbor policies to keep the networks operating, but as they scale, network trust is harder to build and technical solutions must be found.


## Solutions

We see these 6 things as useful tools for helping community networks get started, as well as providing a platform for 

1. **FODD (Federation of Decentralized Documentation):** Establishing lines of contact between mesh locals, document, research, and gather data to be placed in a centralized location and shared with each mesh local.
2. **Mesh-Noc:** Building a stand-alone mesh network operations center that will allow any mesh local (or other decentralized, open-source group) to deploy an open-source productivity and web app suite for everything from emails and calendars, to cloud documents and inter-mesh tunneling. (@mikenabhan) This is in the mesh-noc repo.
3. **Mesh-Stack:** A collaboration, storage, webmail, and office suite for community groups can host their own services. @miknabhan. This does not yet have a repository. Contact one of the devs for access to the test lab instead.
4. **Radio-Lab:** Developing a theoretical framework and test-suite for mesh network spectrum management using anonymous data gathered from librerouters and simulated in the cloud. It will also have tools for building heatmaps of live networks. (@simplymathematics). This lives in the radio-lab repository.
5. **Mesh Map:** Using Raspberry Pis and/or Libre-routers, we will create a heatmapping and spectrum monitoring platform to aid in data collection and analysis for the other components. This also lives in the radio-lab repository. 
6. **Astral Mesh:** Using this new-found inter-mesh network to deploy, test, and rebuild spectrum management techniques like Time Divison Multiplexing and Autonomous Channel State Management (@nicopace). This is an ongoing project across many researchers and institutions. Reach out to him if you would like to be added to the listserv.

## Importance

 The Libre Router project has designed and produced a high performance multi-radio wireless router targeted at Community Networks needs. The reality of the Global South and that of Latin America in particular will be specially considered in terms of cost and legal viability. Further the Libre Router project involves the improvement, the development, the documentation and internationalization of open tools that allow non-technical people to deploy and administrate their community networks based on the LibreRouter+LibreStack platform.

Community networks have proven that it is possible to connect distant, remote, rural or disadvantaged areas to the Internet through radio frequency technology, by allowing people without a high-level of technical skills or resources to deploy their own network infrastructure. This kind of initiatives have been set-up in different places around the world, such as Greece, Nepal, Argentina, Catalonia, India, Ghana, South Africa, Venezuela, Italy, and other countries. They have been growing slowly but steadily, reaching out to people that were not being connected by any type of service provider, be it private or State owned.

AlterMundi, as part of that “network of networks”, has developed over the years a set of tools that have lowered the technical barrier for people to deploy network infrastructure. But there are still some tools that need to be improved, some that need to be built from scratch and some others that need to be documented better in order to allow a bigger audience to take full advantage of this solutions and to reach out to other communities of interest that could potentially deploy community networks in their regions.

Community Networks have been depending since their inception on modifying existing off-the-shelf routers to adapt them to their particular needs.Software development originated in Community Network groups and the Free Software movement as a whole, has pushed the barrier of innovation and helped comercial enterprises develop new products over the years.

This virtuous relation between hardware vendors and the community has been threatened by new regulation from the Federal Communitations Commision (FCC) --which has led vendors to globally close up their routers to third party modifications, hindering open innovation and effectively closing the door to Community Networks in terms of access to the hardware they depend on. In response to this threat to open-source networks, the Librerouter will be shipping its first 2500 units this summer.


[Initial tests](https://github.com/tomeshnet/documents/blob/master/technical/20180530_hpm5g-radio-tests.md) are quite inspiring.

## Methods

There are three key problems facing community networks all over the world right now: documentation and coordination of best practices, parallel reproduction of management/support efforts, and a lack of smart spectrum management. We have a roadmap to begin addressing these issues.

1. Documentation
2. Mesh-Noc
3. Mesh-Stack
4. Radio-Lab
5. Astral-Mesh

## Goals

1. Intermesh book, pdf, webpage, and repo
2. productivity and data center suite for mesh locals
3. mobile spectrum lab
4. Spectrum management tool(s)
5. Rinse, Wash, Repeat


## Team

@simplymathematics: modelling/embedded dev
@mikenabhan: orchestration/deployment

## Data Policies

1. We don't want your data. 
2. Though we are self-funded, all money is tracked  [here](money.thenextbillion.online). Our governance is open-source and _defacto_. Changes to that policy will live [here](meta.thenextbillion.online). 
3. no logs, no masters
4. RSSI, GPS, Link Quality, QoS data
5. Mesh Map Kits
6. Community-controlled spectrum management


## Success

1. FODD
2. Mesh-Noc
3. Mesh-Stack
4. Radio-Lab
5. Mesh-Map
6. Astral-Mesh

## Reproducibility

Github, pdf, book, webpage, peer-review

## Scalability and Federation

Push-button mesh server with extensions, plugins, and/or scripts for extensions for the server stack

## Sustainability

$$$ TBD

### Infrastructure Required:  
##### Checklist  of Infrastructure Required:  

- [ ] ASN  
- [ ] Mesh-NOC  
- [ ] Mesh-Stack 
- [ ] Radio Lab 
- [ ] Organization  
- [ ] Governance
- [ ] Non-Profit Status   

#### BGP/Datacenter Infrastructure:

|Desc| Price |	QTY	 |Total |
|---|-------|--------|------|
|Supermicro E2008D - 128GB ECC RAM	|| $2,300.00 |	1|	$2,300.00| 
|Rackmount Adapter|	 $50.00 	|1|	 $50.00 |
|2TB SSD|	 $300.00 |	2	| $  600.00 |
|ASN| $400| 1 | $400|
|IPv4 adresses (/24) | $4000| /24 | $4000|
|Interconnect Fee | $200 | 1 | $200 |

Total: $7550

#### Server Lab:

|Desc| Price |	QTY	 |Total |
|---|-------|--------|------|
|Intel NUC i5 tall version|	 $  400.00| 	1	 |$  400.00| 
|32GB RAM	| $  400.00 	|1	| $  400.00| 
|2TB SSD	| $  300.00 	|1	| $  300.00| 
|2tb nvme ssd|	 $  600.00 	|1	|$  600.00 |
|Managed Switch|	 $    80.00 |	1	| $     80.00 | 
|Patch Cables	 |$    30.00 |	1	 |$     30.00 |

Total: $1810

#### RF-Lab:  
|Desc| Price |	QTY	 |Total 
|---|-------|--------|------|
|Lime-SDR | $500 | 6 | $3000|
|Libre-routers| $150| 6 | $900|
|Batteries for field test | $300 | 2 | $600|
|Cabling | $100 | 1 | $100|
|Managed Switch |  $100 | 2 | $200 |
| Power Injectors | ~$15| 6 | $100 |

Total: $4900

#### Stipends/Labor:

|Desc| Price |	QTY	 |Total |
|---|-------|--------|------|
| Lawyers, incorporation, non-profit status, and   import/export | $10000 | 1 year | $10000|
|Sprint funds| $20,000| 1 | $20000|
|Research grant| $20,000| for the compilation and federation of community network knowledge in the Americas | 1 year |

Total: $50k

Sprint funds to be allocated based on urgent and widespread need for a given production/deployment schedule as determined by mesh locals. These would be small grants (like $100 for a day of work) that would help us retain 'volunteers' and fund people in the developing world to do important mesh work (where the law permits).  By keeping the grants small and paying by project rather than time, we can open up our development to marginalized communities where $100 would have much more impact without ignoring the very real cost of volunteer labor. The program wil be called developers in diaspora. There are various models to establish a pay scale. Open whisper systems, the developers of signal have a platform for paying per commit to their repository. This might work, but could run afoul of international finance regulations if not done under strict supervision of a qualified attorney.

#### Heat Map Lab:

|Desc| Price |	QTY	 |Total |
|---|-------|--------|------|
Raspberry Pis | $50 | 2 | $100|
Batteries | $60| 2| $120|
GPS modules | $75 | 2 | $150 |
USB wifi dongle | $20 | 2 | $40|

Total: $410

#### Ongoing-costs (2019-2020 Projected):

|Desc| Price |	Term  |Total |
|---|-------|--------|------|
|Translation | $$ | scale | with scale |
|Org Lawyer | $10,000 | annual | $10000 |
|Org Principal (stipend, part-time) | $10,000| annual | $10000 |
|Org support engineers (stipends, part-time) | $40000| annual, scales with member support | $40000|
|Org designer (stipend, part-time)| $10,000| annual | $10000|
|Hosting | $1000 | year | $1000|
|Hardware  maintenance | $10000 | 5 years | $2000/year|
|BGP transit | $.30 | mbps | continuous, with scale |
|Inter-mesh Travel| $200-$500 | per 'local' trip| continuous, with scale |


### Long-Term Funding Ideas:  

 * paid support for librerouters (requires different support model)  
 * grant funding (better as seed capital/not sustainable)  
 * member funding (enough to keep VPS going, not very much labor support at smalls scale)  
* research grants (the big money--labor costs can be funded for new research)  
 * Vpns, tunnels, ip leasing, vps, etc
