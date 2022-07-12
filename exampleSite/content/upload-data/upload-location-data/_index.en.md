---
title: "Upload location data"
weight: 10
date: 2018-12-29T11:02:05+06:00
description: "Create a spreadsheet file with location data, to upload to 4flow NEVA"
---

Once you have [created a project](https://foo.com) you’ll need to add location data to it. You do this by creating a data file in a spreadsheet and uploading it.

## Create a location file
Network Analyzer lets you upload native Microsoft Excel files (\*.xlsx). However, you can use any other spreadsheet program by saving your file in the comma-separated variable (\*.csv) format and uploading that.

When you create this file, you’ll need to use column headers in your spreadsheet file that match the titles listed [here](https://foo.com). For any uploaded file:

* The order of the columns is not important as long as the correct column headings are used
* Only the Key\* column is mandatory; all other columns are optional.

To save time, you may want to download one of the pre-filled templates on the Upload Locations page (see the section [Uploading a location file](https://foo.com)).

## Upload a location file

1.  On your project homepage, ensure **Master data** is selected in the upper tab bar and **Locations** is selected in the lower tab bar. 
    
![Tabs](https://i.imgur.com/3QHYhZ5.png)
    
2.  Press the button **Add or update locations**
    
3.  In the **Upload your data** area of the Upload Locations page, you can drag your file onto the gray pane, or locate the file on your PC by selecting **Select from file**.
    

## Edit location data

You cannot edit location data directly in Network Analyzer. You will need to edit your spreadsheet file and re-upload it.

{{% notice warning %}}
If you re-upload a file with a previously used location key (under the Key\* column), all other details of this location will be overwritten.
{{% /notice %}}

## Delete location data
Deleting locations is not possible—​you must [create a new project](https://foo.com) and upload your updated locations, then [delete the original project](https://foo.com).

## Column headings in data files
Network Analyzer can read data listed under the following column headings in your uploaded file. Please ensure you match the text in your column headings exactly.

: Example spreadsheet file

![Spreadsheet](https://i.imgur.com/mhczSuU.png)

Key*
: Enter a unique key for each location, in line with the protocol of your organization. (This field is mandatory.)

Description
: Enter a description.

Location type
: Enter one of the following types: Supplier; Hub/Cross/Dock; Warehouse; Plant; Customer; Port; Other; Undefined.
: In the Excel template, you can also select these from the drop-down box in the cell.

Postal code
: Enter the postal code.

City
: Enter the city name.

Street
: Enter the street name.

Country ISO2
: Enter the two-letter country code as defined by ISO 3166-1. A list of country codes is [here](https://foo.com).

Country state ISO
: Enter the two-letter country subdivision code as defined by ISO 3166-2. A list of country codes is [here](https://foo.com).

{{% notice note %}}
The Country state ISO is used in the [Bubble](https://foo.com) and [Choropleth](https://foo.com) maps to display regions.
{{% /notice %}}

Latitude
: Enter the [ISO 6709](https://foo.com) co-ordinate for latitude.

Longitude
: Enter the [ISO 6709](https://foo.com) co-ordinate for longitude.

{{% notice note %}}
All locations with unique keys are uploaded to NEVA, regardless of whether there is missing or incorrect information in optional fields. Network Analyzer automatically geocodes locations and fills in missing information where possible; where not possible, it will keep the location and notify you.
{{% /notice %}}