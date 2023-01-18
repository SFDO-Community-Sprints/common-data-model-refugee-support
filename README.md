# Common-Data-Model-Refugee-Support
Common data model for organisations providing support to Asylum Seekers/Refugees


## Use Case
This data model aims to standardise the data capture around support to asylum seekers/refugees. It should enable better collaboration between organisations, as well as reduce admininstration, improve data accuracy, and provide automated support journeys to ayslum seekers/refugees
## Entity Relationship Diagram
![Refugee Support ERD]([Refugee%20Support%20Starter%20Pack%20ERD.png))
## Data Dictionary 
Post an Image of Data Dictionary here
## Installation
Documentation only (apsiration to convert to a package at a later date) 
## Contributing to the Data Model


### Process and Governance 

Common Data Models are Open-Source standardized extensible data schemas that include entities, attributes, semantic metadata, and relationships. While Open-Source, these models try to maximize accessibility by making it an Unlocked Package. When contributing to Common Data Models, the project follow a governance process to ensure it meets all standards.

#### Design-Driven Development
1. Any new Data Model or changes to an existing Data Model will have to go through a review process before being approved for development. 
1. All requests for new features or changes should be first shared in the Trailblazer Community. This is to capture some commmunity feedback on interest as well as some initial requirements.
1. An individual on the Common Data Models Team creates Feature Request Issue in Github following the template, capturing some initial requirements while articulating some expectations.
1. The Feature Request is reviewed by the Common Data Models Team and technical specs are created, adding to the Issue created.
1. The Feature Request Issue is assigned to an individual or a request is made to the community for support on development of the Feature Request.
1. The assigned Developer will document and articulate their solution as part of their process (Create/Update ERD, Data Dictionary).
 #### Development Process
1. Pull *main* branch to get latest updates `git pull origin main`
1. Create feature branch off of *main* branch `git checkout -b feature/issue-key-descriptiveBranchName`
1. Run `cci flow run dev_org --org dev` to create a new scratch org and deploy this project.
1. Run `cci org browser dev` to open the org in your browser.
1. Either develop locally and push to scratch org, or develop in scratch org and pull changes
1. If developing feature in scratch org run `cci task run list_changes --org dev` to see changes that will sync
1. If developing feature in scratch org run `cci task run retrieve_changes --org dev` to retrieve the changes locally.
1. If developing locally, run `cci task run dx_push --org dev` to push local changes to scratch org
1. Add and commit changes to feature branch `git add .` and `git commit -m "issue-KEY: descriptive commit message"`
1. Push feature branch to GitHub and create a pull request to *develop* branch for review `git push origin feature/issue-key-descriptiveBranchName`
1. Delete the scratch org `cci org scratch_delete dev`





