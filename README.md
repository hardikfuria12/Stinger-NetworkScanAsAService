<div style="text-align:center; margin: 50px 0"><img src ="/docs/images/asu-logo.png" height="200"/>

# Stinger : Network Scan as a Service

This project was implemented as part of curricullum for CSE 548: Advance Computer Networks at Arizona State University.

</div>

# Problem Statement 

<p>The first preventive measure taken to cope with Network Attacks, is <b>Network Scan</b>. In this day and age with the rise of Software Defined Networks and IoT-based market devices, we are more prone to various types of security attacks. In this project, we provide Network Scan as a Service for all the devices connected to a given SDN(Software Defined Network).</p>
 
# Proposed Solution
<p>Using, OpenDaylight the open source SDN controller, and OpenFlow communications protocol standard, to control the devices connected to the SDN.
Two types of scan are provided,
 <li><b>Complete Scan</b>: nmap and openvas is used to identify vulnerabilities on services running on ports, and to identify filtered/unfiltered ports.</li>
 <li><b><Custom Scan</b>: provides fine grain scan for specific IP or IP Subnet inputs</li>
 The results of the scan are provided in two formats: XML, JSON. Which is later on consumed by further downstream services</p>
 
# Business Value
This service is of great importance when dealing with real-time network scanning of devices that are set up in a different environment. The ability to scan devices from outside a given environment by leveraging nova and neutron client of the openstack api to manage networking compute instances via the OpenDaylight northbound api, gives greater control over in scenarios of network attacks, research and further downstream analysis.

# Technologies

<li>Flask</li>
<li>OpenDaylight</li>
<li>Openstack</li>
<li>Threading in Python</li>
<li>RESTful Apis</li>

# Drawbacks 
<li>Output of linux command line interface is printed rather than logged or saved. </li>
<li>Lacks Automation scripts to run these services on daily basis rather than current on demand implementation.</li>
<li>Better testing methods other than the implemented honeypot method.</li>
<li>Lacks Bash Scripts to setup the project environment and other dependencies</li>






