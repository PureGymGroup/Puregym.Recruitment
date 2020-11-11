# PureGym IaC test

## Objective

To create simple set of infrastructure resources in azure using Infrastructure as Code techniques.

Please use one of the following tools to create your infrastructure:

- Ansible
- Terraform
- Az CLI / PowerShell

## Requirements

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

## Deliverables

- Clear and readable code with a sensible file structure.
- A simple way to provide credentials to run the infrastructure into our Azure environment
- No software applications need to be deployed to these app services

Feel free to take as long as you feel you need to on this task, we understand that not everyone has a huge amount of time while others feel they want to spend longer to demonstrate everything they can.  We do however ask the task is ideally returned within 7 days of being sent.

When submitting the task please also provide an estimate of how long you feel you spent on the work so we can put the work into context.

You can submit the test in the following ways:
- From a shared link such as drop box, one drive, google drive etc. 
- Shared via a public git repository 

**When sharing via email or a shared link** please zip up your solution with the following name format: [YourNameHere] - BasketTest
