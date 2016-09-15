---
layout: page_collection
title: Step 8 - Identify Common Design Characteristics
permalink: 8_step-8
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

In addition to identifying a solution architecture and the supporting components, you should understand the common design characteristics necessary to successfully implement a modernized PACS. Remember, it’s important to make design decisions that are in line with your agency’s  specific needs and relevant policies.

<br>

| <center>PACS Characteristic ID </center> | </center> PACS Solution Characteristics </center> |
|:----------------------------------------:|----------------------------|
| **PACS 1** | Easily integrated into a centralized management and control system that combines access control with intrusion detection, event monitoring, and integrated video capabilities. |
| **PACS 2** | Supports access to its functionality through both a web-based native user interface and a programmatic application programming interface (API). |
| **PACS 3** | Capable of validating the PIV card in accordance with the authentication mechanisms defined in <a href="http://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-116.pdf" target="_blank"> SP 800-116. </a>
| **PACS 4** | Supports validation of other credential types, as necessary, during migration stages to full PIV card implementation for physical access. |
| **PACS 5** | Provides middleware system(s) that seamlessly integrate the path validation of certificates required by <a href="http://nvlpubs.nist.gov/nistpubs/FIPS/NIST.FIPS.201-2.pdf" target="_blank"> FIPS 201. </a>|
| **PACS 6** | Uses path validation to completely authenticate and validate the security relevant data objects within the PIV card and PIV-Interoperable (PIV-I) cards. |
| **PACS 7** | Provides system components that adhere to the Backend Attribute Exchange (BAE) Specification and are IPv6 addressable. |
| **PACS 8** | Provides a system controller that, with algorithms, will enforce all the rule checks prior to allowing access. |
| **PACS 9** | Adheres to the protocols and architecture recommended in Chapter 10 Initiative 7: Modernization of PACS, requirements. |
| **PACS 10** | Uses PKI certificates as a basis for system administration and visitor management between trusted organizations. |
| **PACS 11** | Included within the Federal Information Security Management Act (FISMA) Inventory of an organization. |
| **PACS 12** | Allows decision making logic to be local, rapid, located within the secure perimeter, and not dependent on a remote server. |
| **PACS 13** | Federated or synchronized with other identity stores that are used for logical access and other aspects of personnel management. |
| **PACS 14** | Consume and process credentials that were produced by authorities independent of the PACS, such as PIV, PIV-I, and facility access cards. |
| **PACS 15** | Read and extract the full Cardholder Unique Identifier (CHUID) from the PIV card, and recognize it within the controllers and server software. |
| **PACS 16** | Allows the PACS server authorization database to update access changes for affected user records in local PACS panels. |
| **PACS 17** | Provides a personal identification number (PIN) entry method to the PIV card. |
| **PACS 18** | Requests and receives the PIV Authentication Certificate from the card, sends data to external PKI infrastructure (Online Certificate Status Protocol [OCSP], Server-based Certificate Validation Protocol [SCVP], Certificate Revocation List [CRL]), and if valid, send to PACS server authorization database. |
| **PACS 19** | Allows the PACS authorization database to integrate to external PKI infrastructure and perform automatic validation of all registered PIV Authentication Certificates. |
| **PACS 20** | Continually checks and updates credential status after the cardholder’s credentials are determined as valid and enrolled in a PACS. |
| **PACS 21** | Provides PACS server software and associated downstream hardware (controllers) that are web services-based in order to allow for more efficient customization to end-user requirements and integration into middleware and external systems components, including Logical Access Control Systems (LACS). | 
| **PACS 22** | Provides a capability to automatically change access level requirements for doors and portals according to preset Threat Condition levels. |
| **PACS 23** | Provides a capability to verify against an internal or integrated external watch list database when a card is presented to a reader for access. Ideally, the watch list should be stored both in the PACS server and controller. | 
| **PACS 24** | Provides a capability to compile reports with data from access records. |























