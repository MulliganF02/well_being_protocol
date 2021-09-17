# WellBeingStudy


Code to run the MIT Month of Wellness Challenge protocol using Reproschema.



### Instructions for making edits
* For each commit, a github action will test the JSONLD code. to know where the error is, you can run the commands in subdirectories.

    ```
    python -m pip install --upgrade pip setuptools
    pip install reproschema requests_cache
    
    reproschema -l DEBUG validate activities
    reproschema -l DEBUG validate protocol/WellBeing_schema
    ```

 


* To display images, click on the image, click on "raw" and copy the URL into the file (e.g., the README-en.md for the landing page). 
    In Markdown: 
    
    `![Timeline](https://raw.githubusercontent.com/danielmlow/WellBeingStudy/master/protocol/wellbeing_logo.svg)` 
    
    
    
When referencing to reproschema-library use the latest commit number




Use the following values for these item responses:
```
            {
                "value": 0,
                "name": "Prefer not to disclose"
            },
            {
                "value": -1,
                "name": "Other"
            },
             {
                "value": 999,
                "name": "None"
             }

```
    



use `clinical_history_psychiatry.includes(-1)` instead of `===` since it is a multiple choice

and use `!clinical_history_psychiatry.includes(-1)` which starts with `!` to show item if it is false. 

