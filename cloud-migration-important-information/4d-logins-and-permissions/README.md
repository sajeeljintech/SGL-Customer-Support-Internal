---
description: >-
  Important information about changes in how logins and permissions are going to
  be handled in the 4D system during the transition to the cloud architecture.
---

# 4D Logins & Permissions

## Linked Logins

The first step in our move to the cloud will be linking logins in the existing system to a valid ShowGroundsLive.com login.&#x20;

The fundamental reason for this is that all existing users will need to be able to login to the cloud system once it launches and that platform will only use SGL logins.

&#x20;&#x20;

{% hint style="warning" %}
IMPORTANT - Linked login must be turned on in customers 4D Systems


{% endhint %}

### Enabling Linked Logins

In EACH 4D system the "Linked Login" preference must be turned on.  To do this open a client to the customer database and login as SG Admin.  Open ShowGrounds Preferences under File->Administration

![](<../../.gitbook/assets/image (75).png>)

Check of "Enable SGL Logins" and click OK.  New users login will be prompted to link their SGL login.



### SGL Login Linking

This process is intruduced during login as a second step to their existing login.  They are prompted for an SGL login.  There are two possibilities here

1. Option 1 - They have an SGL login.  In this case they use it to login AND MUST receive a verification email to confirm that their login for SGL is theirs.  Until this confirmation they will continue to be prompted for the SGL login.
2. Option 2 - They have no SGL login, in which case they must register.

Once a users 4D login has been linked to their SGL login they will only use their SGL login from that point forward.

{% hint style="warning" %}
IMPORTANT - Once a login is Linked permissions are no longer derived from the 4D Group
{% endhint %}

## 4D Groups - After Login is Linked

Once a login is linked permissions no longer come from the 4D Group system but rather from the new group system in the cloud admin. &#x20;
