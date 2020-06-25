# Convert Office documents to PDF

We can use default SharePoint REST API features to convert Microsoft office documents to PDF. SharePoint supports below file types to convert into Pdf.
we can also generate Html from the SharePoint list data and convert into pdf and send in email as a report using this feature
```bash
  "doc",
  "docx",
  "xlsx",
  "xls",
  "ppt",
  "pptx",
  "html"
  ```
### Configure the Flow in your tenant using below steps
1. Download the folder 'Sharepoint files convert to pdf' as a zip package
2. Opent the [Microsoft flow](https://flow.microsoft.com/) site
3. login with your tenant account
4. Go to 'My flows' section
5. Click Import and upload the zip package 'Sharepoint files convert to pdf'
6. You can change the name of th flow and Connections
7. Click on import. Finally it will be imported
8. You can modify the site url, and library name, Site server relative url variables in the flow
9. Save and run the flow using any tools to call http trigger flow
```bash
Post-  <http trigger flow url>
    PayLoad:
    {
    "SiteUrl":"<SharePoint Site url Ex: https://contos.microsoft.com/sites/sitecollection> ",
    "LibraryTitle":"<Library Title>",
    "DocumentID":<Document ID>
    }
```


