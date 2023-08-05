# Common-Charts
___

The common-charts chart controls the deployment of commonly used kubernetes resources via a parent child relationship with
a library charts

## Chart Structure

`./Common/`
* The common chart is used to pull in library charts
  * common/
    * `./Chart.yaml`
      * contains list of library chart dependencies 
    * `./templates/`
      * `./common.yaml`
        * used to import library charts as templates 

`./charts/`
* `./<chartDirectory>/`
  * Contains library Chart.yaml, templates directory, and values.yaml
  
