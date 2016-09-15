---
layout: page_collection
title: Step 6 - Design Solution Architecture
permalink: 6_step-6
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

The FICAM architecture describes the PACS target state as agencies establishing an enterprise approach to managing physical access that links individual PACS via a federated network wherever possible. There are a number of ways to achieve this goal; however your agency should implement a configuration that is cost-effective and aligns with the needs and organizational environment. Physical security staff should also collaborate with IT staff to gain consensus on an appropriate system design, since the Office of the Chief Information Officer (OCIO) has oversight responsibility for ensuring that all IT systems meet relevant requirements. 

Below , you’ll find a high-level example of a solution architecture that encompasses the necessary elements of a modernized PACS. The components represent generic products and are not aligned with a particular vendor or solution offering. Note that several of the items on the diagram, such as Certification Authority (CA) and Authoritative Sources, are common infrastructure components within an agency‘s overall ICAM infrastructure. 

<br>

<div style="text-align:center"><img src="{{site.baseurl}}/img/pacs-arch.png"/></div>

<br>

This diagram represents the target state, in which the PACS is no longer a standalone system. This means the system links into numerous components and provides enterprise physical access authentication and authorization services. The Enterprise Physical Access Infrastructure represents the main services of the PACS and includes critical services like central data storage, monitoring, and control over all of the other components of that system. The enterprise PACS is depicted as a piece of the larger Security Management System (SMS), which has interconnections with other physical security elements such as video surveillance systems, intrusion detection, and fire alarms. 

The Enterprise Physical Access Infrastructure relies on external interfaces to connect with the authoritative sources where relevant user and credential information is stored and maintained. The Enterprise Physical Access Infrastructure administers a variety of field components, which are distributed system components that directly control access at the local level. It’s  anticipated that many agencies will have numerous field components from multiple vendors. In the target state, these devices and subsystems do not necessarily need to be replaced with a single vendor product, but should be linked to an agency‘s PACS services at the enterprise level. 

The diagram depicts an electronic VMS that is integrated with the Enterprise Physical Access Infrastructure. The VMS is an optional element of the physical access solution architecture; however, incorporating an electronic VMS into the enterprise PACS solution may enable additional automation and cost savings. Some agencies may implement a PACS solution in which visitor management is included as a part of the overall system or an agency may choose to develop an independent VMS.

<br>

<div style="background-color: #edf1f3;color: black;margin: 10px;padding: 10px">

<h3><span>FAQ</span></h3>
<p><strong>If the PACS server is hosted by the enterprise and not at my site, how do I know that it is secure?</strong></p>
<p><span>When PACS services are provided at the enterprise-level, servers are hosted at high- security areas with redundant information back-ups, high network availability, and robust disaster recovery protocols. The Service Level Agreement (SLA) for hosting of the system details the security controls and procedures in place. The hosting facility is also subject to Federal Information Security Management Act (FISMA) requirements to ensure adherence with applicable security requirements.</span></p>

</div>












