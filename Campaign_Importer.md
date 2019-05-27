# Campaign Importer

## Purpose of This Guide

This guide describes the method of uploading a campaign file including
the phone numbers to send text messages. It also explains the usage of
the template file used for the importer.

## Campaign Importer

Customers can request callbacks by replying to the text messages
including the keyword specified in the SMS. This works on the basis of a
dialler, but instead of calling, it sends text messages to the contacts
defined in the file.

### How to Upload a Campaign File?

1.  Navigate to ***SMS Campaigns → Campaign Importer***.  
     
2.  Select the company which would like to send text messages to their
    customers.  
     
3.  Choose the campaign file by clicking the **Choose file** button.  
     
4.  Click **Upload** to finish the procedure.

![](attachments/12718798/12718799.png)

![](attachments/12718798/12718800.png)

After the file is uploaded, it  starts to process the records based on
the details provided in the file.

Details, such as:

-   Customer name
-   Phone number
-   Campaign
-   Scheduled Time
-   Any custom data, like reference or account numbers

If there are any messages to be processed immediately, these will be
displayed on the company's wallboard at once.

### Download Template File

The possibility is given to download an empty importer file, so the
administrators can fill the details and upload the file to be processed.

1.  Navigate to ***SMS Campaigns → Campaign Importer***.  
     
2.  Use the **Download Template** button to have the empty sheet.  
     
3.  Fill in the details as described below.  
     
4.  Upload the file. Follow the steps defined above.

#### Elements of the Template File

The template file is a simple excel sheet that needs to be filled with
basic details, such as what phone number to send the SMS or in which
region the customer is located.

The file contains the following columns:

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td>First Name, Last Name</td>
<td>The recipient's name.</td>
</tr>
<tr class="even">
<td>Phone Number</td>
<td>The recipient's phone number. Phone number format is described below.</td>
</tr>
<tr class="odd">
<td>Campaign ID</td>
<td>Specify the identification number of the campaign from which to send the SMS. This can be found on the portal within the SMS campaigns section.</td>
</tr>
<tr class="even">
<td>Region</td>
<td>Specify the region of the customer. This is important to determine the format of the phone number. e.g. <strong>GB,</strong> <strong>IE</strong></td>
</tr>
<tr class="odd">
<td>Fields</td>
<td>Optional fields to include further information on the callback request or any kind of custom data, such as an account number.</td>
</tr>
<tr class="even">
<td>Scheduled Time</td>
<td><p>Specify the time of the message delivery. If the scheduled time is left blank, then the record is processed immediately.</p>
<div>
<div>
<p>Follow this pattern when adding the scheduled time: DD-MM-YR HH:MM</p>
</div>
</div></td>
</tr>
</tbody>
</table>

#### Phone Number Format

Phone Number Lookup

Lookup format used to match the records with the incoming caller number.
Possible values:

-   E164: e.g. +441789387900 (with or without the **+** sign)
-   International: e.g. +44 1789 387900
-   National: e.g. 01789 387900

