# VIBBIO Text content

## Following files are available
 - vibbio.json (in use by both frontend and backend-applications in sprint/development)
 - pubic-pages.json (NOT CURRENTLY IN USE, will be used by frontend-public soon)
 - private-pages.json (NOT CURRENTLY IN USE, will be used be frontend soon)

## Usage of text content

All text content is stored in a json structure with key-value (try to create keys descriptive for the value content).

Text content is displayed with react-intl, mostly `FormattedMessage` or `FormattedHTMLMessage`, sometimes with `formatmessage` directly from `intl` (ex: for getting json-structure to get hold of unknown structure -  quick fix ).

NB! Keys (if correcting) have to be changed in both text content-file and project.

**Prod**

Text content for prod is stored in *vibbio*-bucket in [google cloud storage](https://console.cloud.google.com/storage/browser/vibbio?project=vibbioexpress) in the file *translations.json*.
Make sure to check the file for **public link** after uploading new file. All text content should also be in the master-branch on [Github - translations](https://github.com/vibbio/translations).  
 
**Test/development**
Text content for test/development is stored on [Github - translations](https://raw.githubusercontent.com/vibbio/translations/).
Use the default branch (sprint). 

Make sure the text file is a valid json-file, for example by using [jsonlint](https://jsonlint.com/).

