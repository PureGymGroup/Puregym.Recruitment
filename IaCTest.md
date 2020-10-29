# PureGym IaC test

## Objective

To create simple set of infrastructure resources in azure using Infrastructure as Code techniques.

Please use one of the following tools to create your infrastructure:

- Ansible
- Terraform
- Az CLI / PowerShell

## Deliverables

Please create the following environment:

![IaC test diagram](https://github.com/PureGymGroup/Puregym.Recruitment/blob/master/IaCTestDiagram.png)

- Resource group
- 1 VNet
- 1 app service plan (Please keep size and scale to a minimum)
- 2 app services residing in that app service plan and connected to the vnet
- 1 storage account
- 1 Front Door with routes for both app services
  - A default route going to app A
  - A route for &quot;/AppB/\*&quot; that goes to app B
- 1 WAF protecting the Front Door.

Try to hard code resources as little as possible. Provide enough flexibility that the example could be rerun to create different environments (Alpha, Beta, etc).

## Expectations

- Clear and readable code with a sensible file structure.
- A simple way to provide credentials to run the infrastructure into our Azure environment
- No software applications need to be deployed to these app services

