# Replies

[![image-1714646412469.png](https://doc.puq.info/uploads/images/gallery/2024-05/scaled-1680-/image-1714646412469.png)](https://doc.puq.info/uploads/images/gallery/2024-05/image-1714646412469.png)

[![image-1714646424929.png](https://doc.puq.info/uploads/images/gallery/2024-05/scaled-1680-/image-1714646424929.png)](https://doc.puq.info/uploads/images/gallery/2024-05/image-1714646424929.png)

**Enable Auto-Reply** - Enable this option if you want an automatic reply to be sent upon receiving requests to this department.

<p class="callout warning">**Merge Fields**  
In auto-reply you can enter merge field variables, which the system replaces with the user's data when it sends the reply.  
The exact list of fields you have available in auto-reply message, appears directly below the message box with the field description and merge field code. **Please, be attentive when selecting variables for each response, as specific variables are available for certain types of customers.** Types of customers and lists of available variables:  
**1 Client type -** Registered customer who has chosen the service they are referring to when submitting the inquiry.  
Variables available from the lists : "**Product/Service Related**", "**Client Related**" and "**Other**"  
**2 Client type -** Registered customer who has not chosen the service they are referring to when submitting the inquiry.  
Variables available from the lists : "**Client Related**" and "**Other**"  
**3 Client type -** Unregistered customer.  
Variables available from the lists: "**Other**"</p>

**Overwrite Reply for 1/2/3 Client type** - Enable this option if you want to customize the text of the auto-reply. Otherwise, the Default Reply specified in the Configuration will be sent.

**Reply for 1/2/3 Client type** - Enter the text of the auto-reply for this department. If Overwrite Reply for 1/2/3 Client type is disabled, this message will not be saved, and the Default Reply specified in the Configuration will be sent. Here, you can enter merge field variables, which the system replaces with the user's data when it sends the reply. The exact list of fields available in the auto-reply message appears directly below the message box with the field description and merge field code.

**Select Admin for Auto-Reply** - Specify the admin username for auto-replies. Otherwise, the Default Admin Username For Reply specified in the Configuration will be selected.

**Number of minutes before the reply** - The time after the client's request is created when an auto-reply will be sent. Please note that this time depends entirely on your WHMCS cron job. For example: If a client submits a request at 11:41 and you set this field to "6", and the cron job runs every 5 minutes, then the auto-reply will be sent at 11:50, i.e., in the next cron run. Otherwise, the Default number of minutes specified in the Configuration will be used.

<div id="bkmrk--1"><form class="stretch flex flex-row gap-3 last:mb-2 md:last:mb-6 mx-2 md:mx-4 lg:mx-auto lg:max-w-2xl xl:max-w-3xl"><div><div></div></div></form></div>