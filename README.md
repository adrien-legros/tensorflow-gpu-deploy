# Reference to reproduce the demo

Here are some useful yaml files in order to reproduce the demo presented here: https://github.com/adrien-legros/tensorflow-gpu-demo.

## OpenDataHub

You need to install Open Data Hub Operator through the Operator Hub. Then you will need to create a kind KfDef yaml file to instanciate the ODH components needed. In this example, we will deploy the ODH components in a namespace called *test-odh*. Please refer to the *opendathub/kfdef.yaml* file. Then, in order to deploy the notebook, you will need to create a kind Notebook in your cluster. In order to do so, you can create the *opendatahub/notebook.yaml* file.

## Grafana

We deployed Grafana independently from Open Data Hub in a namespace called *grafana*. You can refer to the Grafana, GrafanaDataSource and GrafanaDashboard files in the *grafana* folder. You will also need to deploy the configmaps associates with the dashboards.