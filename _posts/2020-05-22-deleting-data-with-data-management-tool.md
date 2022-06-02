---
layout: post
title: Deleting data with data management tool
categories: [Data management]
---
### Why?
- You have imported the zip/postal codes incorrectly. Now you want to delete them. However, **you can’t delete them in mass in the form**.
- Or you want to delete data from another table that there is no Excel add-in data connector.

![](/images/deleting-data-with-data-management-tool/image1.webp)

### Option
- Use the setting truncate data entity available in the data management tool.

## Truncating
How does it work?

### 1st – You should create a import data project
When you are creating an import project, there is an option in the *Import* tab called *Truncate entity data*. That field is off by default
> Truncate entity data – control whether all records in an entity must be deleted before an import is perfomed.

![](/images/deleting-data-with-data-management-tool/Image2.jpg)

Once you have created the project and selected the field, the system will display a warning about the impact of this field.
> Choosing to truncate entity data will result in deletion of data in the selected data entities before new data is imported.

### 2nd – You should upload the data file related to the data entity that you want to truncate
There is two option on this step, in my opinion.
- Upload a **data file only with headers** to delete all data on this data entity.
- Or upload a **data file with headers and lines**. First, the system will delete all data. After it will create the new ones present in the file lines.
So to do that you should click on *add file*, select the *entity name*, click on *upload*, and select the data file.

![](/images/deleting-data-with-data-management-tool/Image3.jpg)

### 3rd – Finally, you can import the data file to see the results.
Never do it directly in the production environment.
**First, test it in the UAT environment.**