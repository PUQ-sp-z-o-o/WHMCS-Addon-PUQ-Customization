# Edit Group

#####  [Order now](https://puqcloud.com/whmcs-addon-puq-customization.php) | [Download](https://download.puqcloud.com/WHMCS/addons/PUQ-Customization/) | [FAQ](https://faq.puqcloud.com/)

[![image-1709052855626.png](https://doc.puq.info/uploads/images/gallery/2024-02/scaled-1680-/image-1709052855626.png)](https://doc.puq.info/uploads/images/gallery/2024-02/image-1709052855626.png)

The "Edit Group" page in the ExportTool module is designed to manage and create new groups of data for export. Here's a breakdown of the functionalities available on this page:

\- **Group Name**: This field is where you name your group. It serves as an identifier for the set of data you wish to export.

\- **Secret Word**: Here, you can enter any string which acts as a secret key for generating the hash part of the URL. This is part of the security mechanism to prevent unauthorized access.

\- **Access IP**: This field determines which IP addresses are allowed to access the exported data. You can list multiple IPs separated by commas or use "0.0.0.0" to allow access from any IP. Note that changing this will also change the generated link, as the access IP is factored into the hash generation.

\- **Tables for Export**: A dropdown menu allows you to select from all available tables in your database. Upon selection, all the attributes (columns) available in that table are displayed. You can check the attributes you wish to export, which will then be reflected in the "Visual Tables for Export" section.

\- **Where Condition**: This interactive field allows you to input 'WHERE' conditions that work like 'AND' for each value entered. This feature enables you to refine your data selection based on specific criteria.

\- **Visual Tables for Export**: Displays all the tables you've selected for export along with their attributes and 'WHERE' conditions. In this section, you can see the generated link for data access, copy it, or remove tables from the export group.

To finalize your settings, use the "Save Changes" button. This will update the configurations, including the unique URL generated for data access based on the secret word and access IP you've provided. Remember, each change you make will potentially alter the unique URL, so it's essential to save only after finalizing your settings to ensure consistency and security.