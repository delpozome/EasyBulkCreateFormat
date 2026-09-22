# EasyBulkCreateFormat
This tool facilitates the cross walk between a feature and the bulk create format. It creates 3 outputs: sf_point (or sf_line/sf_poly), tbl_sf_visits and tbl_sf_references. It can be used in conjunction with the Pennsylvania’s Bulk Load Prep Toolbox.  

Install 

You can find the latest code in this GitHub page. To install the tool, follow these steps in ArcGIS Pro:  

Go to catalog > Right click Toolboxes > New Python Toolbox 

 

Delete the prepopulated writing. Copy and paste the code. 

Save 

Prerequisites for using the tool: 

Minimum requirements to use the tool: UniqueID (you can also use ObjectID) and EST_ID. If adding visit/reference information, be sure to have reference_id (not reference code) available to crosswalk. 

The input feature must be projected correctly, especially if using Pennsylvania's Bulk Prep Tool afterwards.  

Using the tool 

Open the tool. Select the feature you’d like to bulk upload and cross reference as many sections as you can. 

Notice: the tool will reformat dates to yyyy-MM-dd.  

 Make sure to QC the output.  

# Best Practices 

When importing data from an excel file, transform it to .csv first and only open it in pro. This prevents pro from truncating text. 

Make sure you are using the correct projection in both the map and the feature, especially if you are using the Pennsylvania tool. 

You can always add extra info to the visit note such as global ID or sbb rule to have at hand when you go back through each SF to make final edits. 
