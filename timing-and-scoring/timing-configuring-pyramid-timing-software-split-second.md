# Timing - Configuring Pyramid Timing Software (Split Second)

## **Overview**

Pyramid timing software uses the SGL Version 1 API for sending live data to the SGL database.  The software supports the following services

1. Live Class View with live timing and score data
2. Live Scoreboard Display
3. GetClass – **This feature does not work as of this writing due to bugs in the Pyramid implementation.**

## **Configuration**

To setup V1 API Access for a particular show company database please read and follow the steps in this document

{% hint style="info" %}
**IMPORTANT - You must do the initial setup instructions below.  This is only needed once per show company but if the Show Company is new to us then the next link must be followed!**
{% endhint %}

### Step 1 - Perform Basic Confirguration for Server to respond to requests

[SGL Timing API Version 1 Setup Instructions](sgl-timing-api-version-1-setup-instructions.md)

### Step 2 - Obtain URL

Obtain URL for Reaching the 4D Based API's - This can be found by going to the RingConfiguration page

1. [https://showgroundslive.com/admin/RvsRingConfiguration](https://showgroundslive.com/admin/RvsRingConfiguration)
2.  Switch to the show company in question

    ![](<../.gitbook/assets/image (108).png>)
3. Obtain the address from the "Web Access" portion of the 4D Server Information group.\
   ![](<../.gitbook/assets/image (106).png>)

### Step 3 - Configure Pyramid

Once that is complete, the remaining setup can be completed in Pyramid software

1. In pyramid software click on the “Header” tab. &#x20;
2. Find the Section labeled “Data to ShowGrounds software”.&#x20;
3. Enter URL  obtained in [Step 2](timing-configuring-pyramid-timing-software-split-second.md#step-2-obtain-url)&#x20;
4.  Enter token which would be obtained in [Step 1](timing-configuring-pyramid-timing-software-split-second.md#step-1-perform-basic-confirguration-for-server-to-respond-to-requests).  See the example below.  Next enter the token obtained in step 2 above.  IMPORTANT: Make sure to check the checkbox labeled “Send data to site”

    ![](http://docs.showgroundsonline.com/wp-content/uploads/2020/08/img\_5f35ae80c05cd.png)

## **Live Scoreboard Operations**

For real time timing data used on the live page and for graphics data must also be sent to our Scoring Server (SRN).  This server handles real time data more efficiently and is used whenever live data is being presented on live class page or for any form of graphics (Scoreboard, Lower 3rd, Leader Board, etc)

To set pyramid to send data to the SRN server follow these steps

1. Obtain the IP address of the computer that is acting as the **SGL SRN Server (Score Routing Node)**The simplest way to obtain the IP address of the SRN server is to visit the Ring Settings page in the admin area for a show company.  This url is typically\
   [https://showgroundslive.com/admin/RvsRingConfiguration](https://showgroundslive.com/admin/RvsRingConfiguration)\
   \

2.  Click on DAK Control.  Enter the IP address obtained in step 1 and port “12345”.  Also be sure to check the “Send via UDP” check box.

    ![](http://docs.showgroundsonline.com/wp-content/uploads/2020/08/img\_5f35b077a8ec2.png)

&#x20;

### **Input Mapping Details**

Assuming they have 4 inputs in the timer. In the input mapping do the following

1. Input 1 to Photocell A
2. Input 2 to Photocell B
3. Input 3 to Photocell C
4. Input 4 to Stop/Restart   (button for the judges to Start/Stop countdown and Stop/Restart timing)

Make sure the box that says “Combine Countdown with Stop/Restart” is checked.

## **Downloads**

If you do not currently have Pyramid software you can download it here.

[https://www.splitsecond.com/software/Equestrian\_Install\_3\_34.exe](https://www.splitsecond.com/software/Equestrian\_Install\_3\_34.exe)

[http://www.SplitSecond.com/software/EquestrianCompanion\_1\_02.exe](http://www.splitsecond.com/software/EquestrianCompanion\_1\_01.exe)
