---
description: >-
  Guide to diagnosing issues with connection for customers to our Remote Desktop
  environment for Cloud Hosted Customers (BELLUS)
---

# Remote Desktop & VPN Trouble Shooting

## Overview

Accessing our Remote Desktop environment is done through a combination of having a live VPN connection to our Bellus Road server network and an active Remote Desktop Connection.  This guide aims to help you determine where a problem may be when a customer is having various issues with their access.//

### Basic Troubleshooting

troubleshooting steps to quickly diagnose and resolve issues that customers may encounter when accessing your software through  Remote Desktop environment protected by a VPN.

#### Level 1 Support&#x20;

1. **Basic Checks:**
   1. **Internet Connection** - Verify that the customer is connected to the internet. \
      You could ask them to be certain they can perform a search at google for instance
   2. **VPN Connected** - Check if the VPN client is connected and showing a stable connection.
   3. **Remote Desktop** - Ensure that the Remote Desktop software is running on the customer's device.
   4. **All Users or Just One** - Determine if the issue being reported is for a single user or all the users at the customer site.  Issues for a single user point strongly to something on that users computer only and not on the network as a whole.
2. **VPN Connectivity:**
   1. Instruct the customer to check their VPN connection status. If the connection is unstable or disconnected, guide them to reconnect.
   2. Verify that the VPN client is configured correctly and is connecting to the correct VPN server.\
      \

3. **Network Speed and Stability:**\
   Ask the customer to perform a speed test using a reputable online tool to check their internet speed.
   1. Go to google and type Speed Test.  Run googles built in test
   2. Ideally >=10 Mb/s download >=5 Mb/s upload or better
   3. Inquire if there are any other devices on the network consuming excessive bandwidth that could be affecting the connection.
      1. Example - Video streaming on the same network connection

#### Level 2 Support

At this point you likely want to involve someone in Level 2 support.

1. **Firewall and Security Software:**\
   Check if the customer's firewall or security software is blocking the VPN connection or Remote Desktop protocol.
   1. Guide the customer to temporarily disable firewall or security software for testing purposes (if safe to do so).  Examples of these tools might include
      1.
2. **Router Configuration:**
   * Inquire about the customer's router configuration and settings. Check if any specific ports need to be opened for VPN or Remote Desktop connections.
   * Suggest restarting the router to refresh the network connection.
3. **ISP Issues:**
   * Ask the customer to contact their Internet Service Provider (ISP) to check for any service outages or network issues in their area.
   * Recommend contacting the ISP for further troubleshooting if the issue persists.
4. **Remote Desktop Protocol (RDP) Settings:**
   * Verify that the customer is using the correct credentials to connect to the Remote Desktop server.
   * Ensure that the Remote Desktop server is accessible and properly configured to accept incoming connections.
5. **Documentation and Logs:**
   * Encourage the customer to provide any error messages or logs they receive during the connection process for further analysis.

By following these troubleshooting steps, we can efficiently identify and resolve connectivity issues that customers may face when accessing our software through a Remote Desktop environment protected by the VPN. Remember to document successful resolutions for future reference and to continuously update your troubleshooting guide with new insights and solutions.

**VPN -** The VPN connection is established by user for access to their remote desktop session. VPN must be installed, logged into, and turned on for any RDP conenction to be established to our in house hosted RDP server. (ProxMox)

**Remote Desktop -** To sign into the session where they can reach the client, users my establish their remote desktop connection. This is assigned to them when their users are added by SGL support staff on the RDS server in the active directory.

**Client Connection -** This is the log in connection to 4D to the client database which is the user's SGL Log in now that everoyne is linked.

**Checking Customer VPN Status:**If a client is experiencing issues with their VPN Connection we can check status here: [http://vpn.showgroundsonline.com/admin](http://vpn.showgroundsonline.com/admin)



## Trouble Shooting Examples

### Sonoma Horse Park - 5/15/2024

**Complaint - EVERYTHING is slow when connected to the VPN**

&#x20;Lyn Nelson reported that her VPN being on creating a very laggy experience. When she has the VPN turned on her machine and network are all VERY slow but when VPN is off everything works as it should, however she then can no longer reach the server or database that she needs for the show.**Fix:Future Diagnostic Questions/References:**

* Run a speed test and get us the screenshot of the reuslts
* Are you ON SITE - Lyn ended up NOT being on property

**Date:** 05/08/2024**Customer:** Blenheim**Issue:** Retha (only her, not multple users) kept being booted out of her RDP session every so often. We enlisted the assistnace from Josh & Desmond & Wes to diagnose and correect the issue**Fix:** Change of the subnet network (IP addaresses)**Future Diagnostic Questions/References:**

* What is your IP Address?
* What type of machine are you on?
* When did this start happening/ when is the last time you got booted out?
* Is this just your machine or multiple users?

​
