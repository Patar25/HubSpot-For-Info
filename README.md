Some basic commands for HubSpot CMS CLI:
----------------------------------------


Setting up local development - https://developers.hubspot.com/docs/cms/guides/getting-started
HubSpot CLI documentation - https://developers.hubspot.com/docs/cms/developer-reference/local-development-cms-cli

- Creating a project:
hs create website-theme my-website-theme

- upload your project:
hs upload --portal=<portal> <src> my-theme
hs upload my-website-theme my-website-theme
(This uploads your project called "my-website-theme" to a folder called "my-website-theme" - first variable is the project, second is the folder)

- watch command:
hs watch --portal=<portal> <src> my-theme
hs watch my-website-theme my-website-theme
(every time you save your file, it will be automatically uploaded)
  
- fetch a project:
hs fetch --portal=<name> <src> <dest>
hs fetch --portal=Patrickod my-website-theme my-website-theme
(You must do this every time you watch to work with files in HubSpot and then run the watch command)

- If you want to upload the watched directory when watch starts:
hs watch <src> <dest> --initial-upload
hs watch my-theme my-theme --initial-upload
