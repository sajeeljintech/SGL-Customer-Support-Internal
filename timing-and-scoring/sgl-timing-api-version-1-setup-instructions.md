# SGL - Timing API - Version 1 - Setup Instructions

## **Overview**

Version 1 of our live timing API utilizes a simple HTTP GET call using URL based parameters to “submit” the data.  This API is handled through the main SGL onsite database server using its built-in HTTP server.  This API provides functionality to

1. Live Class View with live timing and score data
2. Live Scoreboard Display
3. Ability for timing software to “pull” class list.

## **Configuration**

To configure this API you need a few pieces of information.  If you do not have answers to these questions contact ShowGrounds staff to assist.

1. Enable GetTrips API - By default this is not enabled.  To enable it go to the server that hosts the ShowGrounds/4D Database. &#x20;
   1. Use ShowGrounds Client to access the database
   2. Open the Devices module from the Palette.\
      ![](<../.gitbook/assets/image (98).png>)
   3. Look in Devices for a device with the type "Trips Updater API"\
      ![](<../.gitbook/assets/image (112).png>)
   4.  Open this record and find the “Key” value. IMPORTANT – If this device record does not exist create one so that it looks like below.  Token can be set to any value and will need to be used in a later step.

       ![Get the Token - This value is case senstive and must be copied exactly](http://docs.showgroundsonline.com/wp-content/uploads/2020/08/img\_5f35ad9758cd5.png)
2.  Enable GetTrips API - This step must be completed in order for the timing software to be able to retrieve class details from the system\


    1. From the client access the "Administration" menue\
       ![](<../.gitbook/assets/image (96).png>)
    2. Open ShowGrounds Preferences\
       ![](<../.gitbook/assets/image (110).png>)\

    3. Enable Get Trips API\
       ![](<../.gitbook/assets/image (111).png>)



