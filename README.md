---
title: Overview  
---
![](docs/assets/markdown-img-paste-20190526134628192.png)

Version 3.1.1

[[Download PDF version of this document]](Overview.pdf)  

The DigitalPersona Access Management API provides a comprehensive set of components and libraries exposing various functions and methods for using the power of the DigitalPersona platform in your own custom-built native and web-based applications. Sample programs are also provided, which illustrate the features available through the included APIs.
This developer guide is divided into three major sections, not counting this chapter, that align with the specific uses of the various API subsets for supported features and platforms. These sections are

<table style="width:70%;margin-left:auto;margin-right:auto;">
  <tr>
    <th style="width:100px">Section</th>
    <th>Purpose</th>
  </tr>
  <tr>
    <td valign="top" >REST APIs</td>
    <td>Used for implementing credential enrollment and authentication for web-based applications.</td>
  </tr>
  <tr>
    <td  valign="top">Native API</td>
    <td> Used for implementing user authentication for Windows applications. Credential enrollment must be performed using a DigitalPersona client or the Attended Enrollment or Web Enrollment application.</td>
  </tr>
</table>


Through either the REST or Native APIs, you can enroll and authenticate DigitalPersona users quickly and easily against authentication policies as defined by the DigitalPersona administrator or custom policies defined by your application, and subsequently release their users’ protected data (secrets).

All of the authentication credentials provided in the DigitalPersona solution are supported through the corresponding APIs except for the Face credential (for web APIs) and the Bluetooth credential (web and Windows APIs).

### Working environment
Use of the included APIs assumes that an appropriate DigitalPersona solution has been installed, configured and verified. Features exposed through the Native APIs can be used in a minimal DigitalPersona environment consisting of the DigitalPersona Workstation or DigitalPersona Kiosk and a single DigitalPersona AD or LDS Server. Use of the REST APIs requires the additional installation of the DigitalPersona Web Components package.

### Target Audience
Developers should have an understanding of the core components of the DigitalPersona solution and its terminology and concepts. They should also be knowledgeable in the specific target platform and the relevant development language.

## Additional Resources
You can refer to the additional resources described in this section to assist you in using the API.  

<table style="width:100%;margin-left:auto;margin-right:auto;">
  <tr>
    <th style="width:50%">Subject</th>
    <th>Resource</th>
  </tr>
  <tr>
    <td valign="top" >Concepts, features, processes and terminology used in DigitalPersona solutions</td>
    <td valign="top">DigitalPersona AD and LDS Administrator Guides, Client Guide and supporting documentation is available at: <A HREF="https://www.crossmatch.com/company/support/documentation">https://www.crossmatch.com/company/support/documentation </A></td>
  </tr>
  <tr>
    <td valign="top">Concepts, features, processes and terminology used in DigitalPersona solutions</td>
    <td valign="top">DigitalPersona AD and LDS Administrator Guides, Client Guide and supporting documentation is available at: <A HREF="https://www.crossmatch.com/company/support/documentation">https://www.crossmatch.com/company/support/documentation</A></td>
  </tr>
</table>

## System Requirements
### Development system
#### Native API
The recommended minimum software requirements needed to develop applications with the DigitalPersona Native API are:
* Development workstation running Windows 7 or later and DigitalPersona Workstation or Kiosk.

* To compile the sample code: Visual Studio 2008 or later.
DigitalPersona Server running Windows Server 2012 and DigitalPersona AD or LDS Server.

* DigitalPersona Server running Windows Server 2012 and DigitalPersona AD or LDS Server.

See the topic Supported DigitalPersona Products below for a complete list of compatible DigitalPersona clients and servers.

#### REST APIs
In addition to the requirements listed above, the following are required for use of the Web AUTH and Web Enrollment APIs.

* Windows Web Server (IIS)

* DigitalPersona Web Management Components

* An SSL certificate

See the DigitalPersona Administrator and Client Guides for instructions on installing and configuring the above components.

### Target system

Recommended minimum software requirements are the same as for the development system with the following exceptions:

* Visual Studio is not required.

* DigitalPersona Server running Windows Server 2012 and DigitalPersona AD or LDS Server.

* If the logon and Password Manager features are not needed, the DigitalPersona client can be installed without these applications. This installs the DigitalPersona Access Management API runtime only.

## Supported DigitalPersona Products

The DigitalPersona Access Management API is compatible with the following DigitalPersona products:

* DigitalPersona AD or LDS Workstation 2.1 or later.

* DigitalPersona AD or LDS Kiosk 2.1 or later.

* DigitalPersona AD or LDS AD Server, version 2.1 or later.
