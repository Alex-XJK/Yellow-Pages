# Yellow-Pages
A sample web page for easy creation of a personal website yellow page

## Disclaimer
> Initially designed for my friend, Y.H. DING.  
> The code skeleton was adapted from my toolsweb page in my personal homepage, which was already deployed in 2019.  
> I was only responsible for the code design of the website, the content of the links and the deployment and management of the website were all handled by the forked sub-project owners.  
  
## Steps
- `fork` this repo to your own account.
- Configure GitHub Page settings or personalize other static site deployment processes.
- Edit the `~/config.json` in the home directory.
- Go to your deployed page or refresh the page to see the latest updates ( based on different caching server or client browser properties, you may have to wait up to several minutes to avoid resource caching).

### config.json
The hierarchy and the required keys in json are shown below. You can have an infinite number of sections, and an infinite number of links under each section, while keeping the format, keys, data types, and other information in line with the requirements.  
```json
{
    "section": [
        { 
            "header": "<The title of your first block>",
            "content": [
                {
                    "title" :  "<The displayed title for your link 1-1>",
                    "url"   :  "<The actual page URL 1>",
                    "msg"   :  "<The optional hover message or description of your link>" / null
                },
                {
                    "title" :  "<The displayed title for your link 1-2>",
                    "url"   :  "<The actual page URL 2>",
                    "msg"   :  "<The optional hover message or description of your link>" / null
                }
            ]
        }, 
        { 
            "header": "<The title of your second block>",
            "content": [
                {
                    "title" :  "<The displayed title for your link 2-1>",
                    "url"   :  "<The actual page URL 1>",
                    "msg"   :  "<The optional hover message or description of your link>" / null
                },
                {
                    "title" :  "<The displayed title for your link 2-2>",
                    "url"   :  "<The actual page URL 2>",
                    "msg"   :  "<The optional hover message or description of your link>" / null
                }
            ]
        }
    ]
}
```

### layouts
The user-editable style file is located at `~/source/basic.css` and supports the standard css syntax format.   
By default, when the page is presented in landscape, the link entries in a section will be laid out in up to 4 columns, but in portrait, the layout will revert to the single column.

## Footnotes
Latest updated on Sept. 23, 2022 (EDT) by Alex XU.
