# Module TF_DO_PROJECT

Module responsible for creation of project in Digital Ocean using Terraform.

## How to use

You need first clone this repo in you project or use this as module in your git repo.

For creation, you just need pass 4 variables:

```bash
module do_project {
  source = "../modules/tfdo_project/" # Path to module
  
  project_name = "seu-madruga" # Project Name
  project_description = "Project for miscellaneous apps used daily" #Project description
  project_purpose = "Other" # Project purpose
  project_environment = "Production" # Project Environment
}
```

And after creation the __Project ID__ will be output for usage by others modules.

