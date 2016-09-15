---
layout: page_collection
title: Step 4 - Review Solution Components
permalink: 4_step-4
---
<script>
$(function() {
  $( "#accordion" ).accordion({
    heightStyle: "content",
    collapsible: "true",
    active: "false"
  });
});
</script>

<script src="https://use.fontawesome.com/e20c671b68.js"></script>
-----------------------------------------------------------

After you’ve reviewed the diagram that shows the many components that comprise an enterprise PACS solution, you can learn more in detail of the functionality of each component. See below to learn more about in detail about the components that make up the Enterprise Physical Access Infrastructure.

<div id="accordion" markdown="1">

### PACS Server
<div markdown="1">

The PACS server is an administrative tool used by the PACS operator to provision and de- provision access to a variety of physical resources, control and configure downstream access control and alarm devices in the system, journal all system activities, and execute security- related decisions. The PACS server is also typically the primary data source where a cardholder is enrolled or registered in the Cardholder Database. 

<br>

<div style="background-color: #edf1f3;color: black;margin: 10px;padding: 10px">

<h3><span>Implementation Tip</span></h3>
<p><span>PACS servers can be managed by the agency at the enterprise level or by a service provider using cloud computing approaches. This model, called Security-as-a-Service, involves a technology provider hosting the security management applications on behalf of the end user. This arrangement allows agencies to leverage the cost savings, flexibility, and ease-of-deployment and eliminate the server and storage infrastructure at each individual site.</span></p>

</div>
</div>

### Workstation
<div markdown="1">

The workstation is subordinate to the PACS Server and provides administrative functions to manage the PACS. In an enterprise network with a network-centric PACS, a workstation can be placed where needed and connected to the network in order to operate in conjunction with the PACS Server. Some of the typical functions controlled at a workstation are adding or removing cardholders and credentials from the PACS, downloading cardholder data, and setting access levels and functions of the field components. They may leverage thin clients using browser interfaces only, or use thick clients that use locally installed software.

<br>

<div style="background-color: #edf1f3;color: black;margin: 10px;padding: 10px">

<h3><span>Implementation Tip</span></h3>
<p><span>Close coordination with network administrators is required to successfully integrate workstations as part of the PACS solution. PACS implementers should coordinate with IT resources to help determine workstation location and set up network connectivity.</span></p>

</div>
</div>

### Controller/Panel
<div markdown="1">

The controller/panel makes access control decisions by comparing cardholder data sent by the reader with the cardholder data stored locally. The controller/panel contains a number of cardholder records, usually one per cardholder, which typically consists of a cardholder record number, a cardholder photograph, a unique identifier (card number), a list of authorized access points, and a time when access is authorized. The decision to grant access is based upon successfully matching the cardholder data with an existing record and its associated access privileges. 

There are some PACS that operate without a controller/panel by connecting a variety of standard reader types directly to a network through Internet Protocol (IP) bridges. This type of architecture might typically be found in PACS architectures leveraging a Security-as-a-Service model.

</div>

### Card Reader
<div markdown="1">

A card reader is the device located at an access point to provide access control. A card reader may support communication with either the contact or contactless interface of the card, or in some cases support both. A  card reader should also support bi-directional communications with the system, processing the data and instructions from the card, sending the data to the associated control panel, and receiving data and instructions back from the control panel within an acceptable time frame.

It is likely that a card reader will need to read and communicate various data from the card in order to support transactions that use multiple authentication modes, including Cardholder Unique Identifier (CHUID) and PKI authentication. When you begin to select card readers for your agency, it’s important to ensure that the card reader chosen is capable of supporting the desired PIV card authentication mechanisms at a particular access point, as not all card readers support all authentication mechanisms.

<br>

<div style="background-color: #edf1f3;color: black;margin: 10px;padding: 10px">

<h3><span>Implementation Tip</span></h3>
<p><span>Ensure that environmental factors are taken into consideration when designing your agency’s PACS, particularly when deciding what types of card readers to purchase. Environmental factors, such as exposure to weather conditions, can impact the successful use of a card reader through the contact mode. An agency may need to deploy additional equipment, such as a protective cover, in these scenarios.</span></p>

</div>

<br>

It is likely that a card reader will need to read and communicate various data from the card in order to support transactions that use multiple authentication modes, including Cardholder Unique Identifier (CHUID) and PKI authentication. When you begin to select card readers for your agency, it’s important to ensure that the card reader chosen is capable of supporting the desired PIV card authentication mechanisms at a particular access point, as not all card readers support all authentication mechanisms.

<br>

<div style="background-color: #edf1f3;color: black;margin: 10px;padding: 10px">

<h3><span>Implementation Tip</span></h3>
<p><span>When selecting to use an “edge reader” or “Internet Protocol (IP) reader,” it is suggested that agencies choose the two part variety. This ensures that the controller function and IP port are located on the secure side of the wall, opposite the reader.</span></p>

</div>
</div>

### Cardholder Provisioning System
<div markdown="1">

A Cardholder Provisioning System is an example of an external interface that integrates between a PACS and an agency‘s authoritative identity source(s) to provision user accounts and their associated card data to the PACS. The use of a Cardholder Provisioning System represents a shift in the target state, where the PACS is a consumer of identity and PIV credential information. 

</div>
</div>



















