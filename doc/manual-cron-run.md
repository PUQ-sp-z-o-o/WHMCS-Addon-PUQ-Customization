# Manual Cron Run

Manual Cron Run extension provides users with the ability to manually execute cron jobs.

# Description

The "**Manual Cron Run**" extension is a powerful tool that offers users the flexibility to manually execute various cron jobs. With this extension, you can take control of your website's scheduled tasks and ensure they run exactly when needed. Here are the key features of the "**Manual Cron Run**" extension:

1. Manual Execution of Daily Cron: With this feature, you can easily initiate the execution of the Daily Cron job at any time you desire.
2. On-Demand System Cron Execution: The extension allows you to run the System Cron job on-demand. By manually triggering this essential task, you can ensure that critical system-level processes and maintenance tasks are executed promptly and efficiently.
3. Run Specific Cron Jobs from the Table: The "**Manual Cron Run**" extension offers a comprehensive list of cron jobs, presented in a convenient table format. From this list, you can handpick specific cron jobs that need immediate attention and execute them individually.

By giving you the power to manually run cron jobs, the "**Manual Cron Run**" extension provides unparalleled control over your website's backend processes. You no longer have to wait for the scheduled cron execution, as you can initiate these tasks at your convenience.

It does not disrupt your regular cron setup but rather enhances it by providing additional control and management options.

Manual execution of cron jobs enables you to closely monitor their performance and ensure that they complete successfully. If any issues arise during the execution, you can promptly address them, keeping your website running smoothly.

By enabling manual triggering of Daily Cron, System Cron, and specific cron jobs from a user-friendly interface, this "**Manual Cron Run**" extension becomes an indispensable tool for optimizing your WHMCS website's performance and efficiency.

# Configuration

[![3.png](https://doc.puq.info/uploads/images/gallery/2023-07/scaled-1680-/zOT3.png)](https://doc.puq.info/uploads/images/gallery/2023-07/zOT3.png)

### **PHP Binary File**

First, find out the version of PHP and ionCube on your WHMCS. You can do this by navigating to Utilities -&gt; System -&gt; PHP Info.

[![4.png](https://doc.puq.info/uploads/images/gallery/2023-07/scaled-1680-/4.png)](https://doc.puq.info/uploads/images/gallery/2023-07/4.png)

It is crucial that your ionCube version is v12 and above; otherwise, our extensions will not function correctly.

After determining the PHP version of your WHMCS and ensuring that your ionCube is v12 and above, you need to find out where the PHP binary file is located on your server. To do this, run the command "**whereis <span style="color: #ff0000;">your\_php\_version</span>**" in the console, replacing "<span style="color: #ff0000;">your\_php\_version</span>" with your PHP version:

[![6.png](https://doc.puq.info/uploads/images/gallery/2023-07/scaled-1680-/6.png)](https://doc.puq.info/uploads/images/gallery/2023-07/6.png)

When entering this path in the configuration menu of this extension, make sure it is correct. If the path is incorrect, the extension will produce an error, and you won't be able to continue working with this extension:

[![7.png](https://doc.puq.info/uploads/images/gallery/2023-07/scaled-1680-/7.png)](https://doc.puq.info/uploads/images/gallery/2023-07/7.png)

### **Crons List**

You can find a complete list of available crons in the official WHMCS documentation ( [Task Options for skip and do](https://docs.whmcs.com/Crons#:~:text=the%20respective%20invoices.-,Task%20Options%20for%20skip%20and%20do,-When%20performing%20a) )

To activate a specific cron, all you need to do is click on "Run Cron Now," confirm the request to execute the cron, and wait until the loader disappears and redirects you to another page.

[![8.png](https://doc.puq.info/uploads/images/gallery/2023-07/scaled-1680-/8.png)](https://doc.puq.info/uploads/images/gallery/2023-07/8.png)

[![9.png](https://doc.puq.info/uploads/images/gallery/2023-07/scaled-1680-/9.png)](https://doc.puq.info/uploads/images/gallery/2023-07/9.png)

# Search

This page is created for you to control your cron jobs and their outputs.

Here are displayed:

1. Command Name
2. Process/Output of the command
3. Date and time of execution

[![11.png](https://doc.puq.info/uploads/images/gallery/2023-07/scaled-1680-/11.png)](https://doc.puq.info/uploads/images/gallery/2023-07/11.png)

#### Redirecting to the Search page upon activating a cron.

When you manually launch any cron, you will be redirected to the Search page, where all executed cron jobs with the specified name for the current day will be shown.[![10.png](https://doc.puq.info/uploads/images/gallery/2023-07/scaled-1680-/10.png)](https://doc.puq.info/uploads/images/gallery/2023-07/10.png)

#### Viewing the list of completed cron jobs.

You can view the list of any cron job for any day by selecting the date in the form and clicking "Search...". If you want to view all cron job entries, simply select "Any" in the "Choose Cron Task" list.

![12.png](https://doc.puq.info/uploads/images/gallery/2023-07/scaled-1680-/12.png)[![13.png](https://doc.puq.info/uploads/images/gallery/2023-07/scaled-1680-/13.png)](https://doc.puq.info/uploads/images/gallery/2023-07/13.png)

#### Clearing the list of manually executed cron job logs:

To clear the list, simply click on the "Clean Manual Cron Logs" button and confirm the prompt that appears.

<p class="callout warning">When you click the button to clear the list of manually executed cron job logs, **ALL data** recorded in this table about manually executed cron jobs **will be deleted**.  
Please be cautious before performing the deletion.</p>

[![14.png](https://doc.puq.info/uploads/images/gallery/2023-07/scaled-1680-/14.png)](https://doc.puq.info/uploads/images/gallery/2023-07/14.png)

