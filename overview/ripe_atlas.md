## Ripe Atlas Overview

All of this you can go and read yourself, so consider it a quickie TL;DR.

Ripe Atlas can be reached found here: https://atlas.ripe.net/ and if you want to 
read all of the documentation yourself you can find it here: https://beta-docs.atlas.ripe.net/

Ripe Atlas is a global probe network run by the Ripe NCC that is used both by companies, researchers and
private persons.

Based on probes that are hosted primarily by private individuals and Anchors, enhanced probes and targets
for regional measurements, that are often hosted by organisations.


The basic idea is that if you host a probe or an anchor you can earn credits and help the internet community.

You can then if you wish use these credits to run measurements of your own. 

Ripe Atlas is also useful with out even owning a probe or having credits.

<br>
<br>
<br>

	=== DNSMON ===
One 'free' services is the Ripe Atlas DNSMON:


DNSMON is a frontend that presents and overview of DNS measurements that are run on a recurring basis.
* [ ] Present DNSMON
    * https://atlas.ripe.net/dnsmon/group/se. 
    * https://atlas.ripe.net/dnsmon/group/nu.

    
* [ ] Show recurring measurements



### Open Data

There are a lot of measurements that are set up with public results. This is another area where there is 'free' data. You can just download the results, but the best way to access and use this data is via the API's: https://beta-docs.atlas.ripe.net/apis/ 

This is out of scope of this walk through.


## Afer this point you will need a Ripe Atlas account and some credits

Ripe Atlas registration: https://access.ripe.net/registration

### Measurements

Measurements can be set up using both the web-gui and the API's. I can recommend learning to use the API's if you find yourself using Ripe Atlas to make a lot of measurements.


* [ ] Set up a measurement
	From the [measurements](https://atlas.ripe.net/measurements) page click on the "+ Create a Measurement"  [link](https://atlas.ripe.net/measurements/form/).
* [ ] Fill in the form. (The following is a working example)
	* Target:  a.ns.se
	* Address Family: IPv4
	* Query Class: IN
	* Query Type: SOA
	* Query Arguement: se 
	* Description: My really cool atlas measurement
	* Interval: We wont' fill this in since we will do a one off and save a little credits
	* Tags: you know if you have a lot of measurements and have to find them later
	* Use the Probe's Resolvers(s): I almost never use this.
	* Resolve on Probe: same here
	* Set NSID bit: Always set this, it will give you information on what server is answering

* [ ] Probe Selection:
	* If you want to just use worldwide 10 fine otherwise
	* kill that one and click on "New Set Wizard"
	* Write "Sweden" in the "Search by place, IP, prefix ... " field
	* Select the number of probes
	* Add ( Include and Exclude based on tags is outside the scope of this document, go read the docs)
	* OK
	
* [ ] Timng:
	* OK this is important. Choose "This is a One-off" Running measurements can get "expensive", This should cauase the "Cost summary" to reduce drastically.
	 
	  
* [ ] Click on "Create My Measurement"
* [ ] Check out the results
* [ ] You will get a pop up when you created the measurement to access the measurement:
	* Settings & Status
		- an overview of the information used to create the measurement
	* Latest Results
	 	- Gui access to the results from the measurement
	* Map
		- A map of the probes involved in the measurement
	* Downloads
		- You can download the results here for machine parsing 

