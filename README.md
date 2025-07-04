# SharePoint SE Filtered Lookup Field

This is SharePoint SE port of *SharePoint 2010 Filtered Lookup* provided [here](http://sp2010filteredlookup.codeplex.com/) by Dev4Side, which is also a port of the package provided [here](http://filteredlookup.codeplex.com/) :) SharePoint 2013 version can be found [here](https://github.com/hasangok/sharepoint-2013-filtered-lookup-field).

I updated namespaces, pages and SharePoint binaries (to use version 16.0.0.0). Description below is copied from [here](http://filteredlookup.codeplex.com/) and all the features are working perfectly with SharePoint SE.

## Description
This project creates a custom SharePoint lookup field that offers new functionalities to default SharePoint lookup field by allowing filters to be applied to retrieved data. Applied filters can be either dynamic CAML queries or pre-defined list views residing in source lists.

Below is a few of the features offered by Filtered Lookup field over standard SharePoint Lookup field:  
* Cross-site lookup (all sites within same site collection)
* Filter retrieved data using list views
* Filter retrieved data using dynamic/ad-hoc CAML queries. This means you don't need to create a list view each time you want to apply a lookup filter to source data
* Supports retrieving data recursively using either list views or dynamic queries
* Supports MultiLookup with filtered data
* Same look and feel as default SharePoint Lookup and MultiLookup (i.e. in list forms)

## Installation
Download wsp package from [here](https://github.com/FOLDBYTE/Dev4Side.SPSE.FilteredLookup/releases), put it into your SharePoint server machine and run the following commands in *SharePoint SE Management Shell*.
```powershell
Add-SPSolution "/path/to/Dev4Side.SPSE.FilteredLookup.wsp"
Install-SPSolution –Identity Dev4Side.SPSE.FilteredLookup.wsp –GACDeployment
```

## Screenshot
![filtered_lookup_sp2016.png](https://github.com/FOLDBYTE/Dev4Side.SPSE.FilteredLookup/blob/master/filtered_lookup_sp2016.png)
