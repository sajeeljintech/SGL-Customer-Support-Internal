# Timing Integration - Overview - Internal Documentation

## Overview:

Increasingly we are supporting companies that are providing timing services and wanting to integrate with us.  We want the integration with timing so in general the initial integration is something we always want to support.

Once we have integration with the timing software many other things become possible such as live results on the web site, running a live scoreboard, creating lower third graphics and many others.    These services we will be charging for in the near future.

## Types of Integration

We have two basic types of timing integration.  We can think of them as Version 1 and Version 2.

### **Version 1 – Basic Score Data – NO GRAPHICS**

This version communicates directly to the ShowGrounds (4D) Server but only captures “major” events during the time the horse is in the ring, such as faults and final time.  We are not able to run any live video based graphics such as Scoreboards, Video walls, lower third graphics or integration with other graphics systems such as Ross Expression or Caspar.

### **Version 2 – SRN Server – Graphics Enabled**

We must have SRN in place.  At this time will likely be running on the same LAN to receive data and perform necessary functions.  With SRN comes options for HTML based Scoreboard, Singular Scoreboard, Singular Lower 3rd, etc.

IMPORTANT – Currently some customers are paying while others are not.  This will get standardized by early 2023 so that these services are always charged to the customer.  This is to say ALWAYS check with Wes, Sheryl to make sure that the customer is approved for the services to be enabled.

## Basic Timing Software Integration

All of this information is as of 10/12/22 and is likely to change in the not too distant future. This document needs to be updated accordingly.

We currently integrate with 4 timing programs

1. Pyramid Software/Split Second –
   1. ShowGrounds Server (NON-SRN) Direct Integration: YES\
      [Timing – Configuring Pyramid Timing Software (Split Second)](timing-configuring-pyramid-timing-software-split-second.md)
   2. SRN – Yes (using DAK Control)\
      [Pyramid SRN – Setup Instructions](http://docs.showgroundsonline.com/documentation/getting-started/miscellaneous/pyramid-daily-setup-instructions/)
2. RyeGate
   1. ShowGrounds Server (Non-SRN) – Only used for GetClass Operation\
      [Ryegate Scoring – Configuring for communications with SRN](http://docs.showgroundsonline.com/documentation/ryegate-scoring-configuring-for-communications-with-srn/)
   2. SRN – Yes (under Hardware settings)\
      [Ryegate Scoring – Configuring for communications with SRN](http://docs.showgroundsonline.com/documentation/ryegate-scoring-configuring-for-communications-with-srn/)
3. Eagle Eye Chronos
   1. ShowGrounds Server (Non-SRN) – Only used for GetClass Operation
   2. SRN – Yes\
      [Eagle Eye Chronos \&#8211; Timing Integration Set Up](http://docs.showgroundsonline.com/documentation/eagle-eye-chronos-timing-integration-set-up/)
4. Skunkware

## Setting Up Graphics

IMPORTANT – DO NOT DO THIS WITHOUT APPROVAL

1. What Timing Software are they using?  This must get answer first as all setup after this depends upon it.
2. \


\
