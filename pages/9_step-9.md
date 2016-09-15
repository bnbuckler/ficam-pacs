---
layout: page_collection
title: Step 9 - Automated Provisioning to PACS
permalink: 9_step-9/
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
---------------------------------------------------------

Automated provisioning to PACS has developed into an important aspect of consideration for those who manage and maintain those systems. Automated provisioning of an individual‘s digital identity into a PACS helps to address system resource management issues and several overarching security concerns including, but not limited to:

> * Ensuring that an individual‘s user record is based on authoritative identity data;

> * Providing system administrators the ability to better manage their PACS databases and keep records current; and

> * Allowing for centralized and automatic de-provisioning when an individual separates from an agency.

Traditionally, the data elements needed to create an authorized cardholder within a PACS database have been entered manually. In addition, the procedures for determining how someone is granted access are disparate across the government and even within a single agency. This has led to the realization that a set of standard data elements within a digital identity should be available to the PACS for the creation of a cardholder profile. An agency will benefit from the standardization that results from having the PACS populated with an established digital identity from authoritative source(s). 

<br>

<div style="background-color: #edf1f3;color: black;margin: 10px;padding: 10px">

<h3><span>Lesson Learned</span></h3>
<p><span>Take your existing PACS infrastructure into account when selecting an automated provisioning approach. The Department of Health and Human Services (HHS) established the enterprise Credentialing Provisioning and Gateway System, which interconnects the HHS Smart Card Management System to the many stove-piped, proprietary PACS installed throughout HHS. HHS has been able to quickly realize the benefits of automated provisioning while reducing system development costs by leveraging their existing PACS to the maximum extent possible.</span></p>

</div>

<br>

The target state of a modernized PACS is to realize a singular digital identity, which can be added to, modified, and deleted by one or more authoritative data source, as determined by each agency. The complexity of the digital identity is dependent upon the size of the agency, the facilities to be covered, and existing architecture in place to support the effort. The target state should be supportive of a single digital identity being created and maintained at the agency level for distributed cross-system use, a concept commonly referred to in the physical security community as ―single enrollment, many uses. Below, you’ll find commonly available automated provisioning approaches for your consideration. 

<div id="accordion" markdown="1">

### Integrated Provisioning Capability
<div markdown="1">

A fully automated provisioning capability that leverages a real time connector using open standards (i.e., eXtensible Markup Language [XML]) and enables two- way communication between the PACS and authoritative sources.

## <i class="fa fa-thumbs-o-up" aria-hidden="true"></i> &nbsp;<span style="color: #0C5C89">**Benefits**</span>

> * Significantly less level of effort for enrollment to PACS 

> * Minimized development costs

> * Standardized naming conventions

> * Reporting capability

> * Works well if agency has a variety of vendors

> * More options for federation of PACS control into the enterprise

> * Security personnel have assurance that data integrity is maintained across the entire landscape of PACS

> * Provides the connected PACS with the most current cardholder account information, including access privileges

> * Provides a robust and flexible, oftentimes web-based, interface that can access data from the connected PACS in a seamless and intuitive fashion

> * Can function as a central point of revocation of cardholders’ accounts, further increasing an efficient security posture of the organization

> * Maintains connections on a near real-time basis using resource connectors or service interfaces.

## <i class="fa fa-exclamation-triangle" aria-hidden="true"></i> <span style="color: #0C5C89">**Limitations**</span>

> * Often reliant on software vendor after installation for maintenance

> * Must maintain connectivity through real-time connectors or system interfaces to update systems

> * Upgrading software can be costly

</div>

### Vendor Interfaces
<div markdown="1">

Leverages custom scripts written by a vendor using application programming interfaces (API) and software development kits (SDKs).

## <i class="fa fa-thumbs-o-up" aria-hidden="true"></i> <span style="color: #0C5C89">**Benefits**</span>

> * Allows data sharing between two systems on a long-term basis

> * Utilizes existing systems SDKs and vendor expertise

> * May be more open/flexible than batch processing

> * Pre-set schedules/time intervals for the transfer of new data/enrollments

> * Higher level of quality assurance with data integrity during data transfer than offered in the single-use option

> * Many current PACS and some legacy systems provide this option

> * Properly developed scripts are typically functional across a broad range of software versions

## <i class="fa fa-exclamation-triangle" aria-hidden="true"></i> <span style="color: #0C5C89">**Limitations**</span> 

> * Incomplete mapping of cardholder information

> * Real time operation depends on vendor

> * Depending on vendor may require heavy investment

> * Multiple systems would increase complexity in cross-system cardholder record integrity

> * May create inconsistency among systems which can negatively impact security

</div>

### Batch Processes
<div markdown="1">

Leverages a single-use scripted data transfer.

## <i class="fa fa-thumbs-o-up" aria-hidden="true"></i> <span style="color: #0C5C89">**Benefits**</span> 

> * Is easy to implement when transitioning from a legacy PACS to a new access control system

> * Can utilize existing custom infrastructure

> * Minimized effort through targeted scripts based on requirements

> * More flexible to meet particular agency requirements or unique existing infrastructure

## <i class="fa fa-exclamation-triangle" aria-hidden="true"></i> <span style="color: #0C5C89">**Limitations**</span> 

> * May not completely eliminate manual operations as part of provisioning process

> * Complexity may increase database management issues

> * Possible difficulty in validating data transfer

> * Generally used for one-time data transfer

> * No recurring data transfer as data changes in the authoritative source

> * Does not guarantee the quality and uniqueness of imported cardholder accounts

> * A scripted process is generally only functional within a small range of software versions

> * There can be disconnects between the individuals who build the data transfer script and those who are familiar with the PACS system itself

> * A significant time investment may be required to ensure cardholder accounts properly reflect the individuals they are

</div>
</div>




















