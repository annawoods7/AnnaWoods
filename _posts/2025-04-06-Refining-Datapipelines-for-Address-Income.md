---
layout: post
title: "Refining Datapipelines for Address Income"
date: 2025-04-06
---
This past semester I worked as a Data Engineer for [Address Income](https://www.addressincome.com/company/about-us) - a real estate investment firm. During this time I was able to complete wide range of cool projects that brought me out of my comfort zone as an information systems major. 

<div align="center">
  <p>Thank you to Address Income and Nevada Career Studio for hosting this internship!</p>

  <img src="{{ site.baseurl }}/assets/images/NevadaLogo.png" alt="Image 1" width="200" style="margin-right: 10px;">
  <img src="{{ site.baseurl }}/assets/images/AddressLogo.png" alt="Image 2" width="200">
</div>



# Background 
One of the goals Address Income has is to host an online platform that congregates key real estate data into a pleasant user interface everyday investors are able to access. The website will also contain features such as but not limited to: Single family and Multi family analytics reports, varying levels of access for different user types, dashboards, and realtime data updates.

# Projects
This resulted in a variety of projects that I had the pleasure of working on. In this blog, I will focus on the top three: **Data cleaning using Airflow pipelines and python pandas library**, **Setting up Deployment of a Development website through Github Actions**, and **Configuring a Docker compose file for user authentication**. 

Each of these projects was a team effort with my fellow team members Anthony, Rania, and Sean. 

#### Data cleaning using Airflow pipelines and python pandas library
  One of my first projects was to write a python function to clean data coming from a real estate API for insertion into a database hosted in Supabase (a database hosting software). This required:
  
  -  Examing JSON files to determine what data to collect
  -  Mapping column names
  -  Creating cleaning functions for certain columns
  -  Creating functions to convert data into python data types
  -  Debugging code by examing Airflow logs

Pandas dataframes were used to more conveniently reformat data such as column names and values. Below is an example of the airflow tasks logs:

![Airflow Example]({{ site.baseurl }}/assets/images/Airflow_example.png)

#### Setting up Deployment of a Development website through Github Actions
  Later on I was tasked with using Github actions to deploy the react website. This required:

  - Configuring a yaml file in Github workflows
  - Setting up SSH capabilities for Github Actions to write to the company development server
  - Building the react project to be hosted on the developmnent server

  The workflow looks something like this:

  ![workflow_Example]({{ site.baseurl }}/assets/images/deploy_web_diagram.drawio.png)



#### Configuring a Docker compose file for user authentication
  My final, and currently ongoing, project is to configure a Docker compose file which authenticates users. This will ensure access to view the development website is secure and only alotted to the proper users. This requires:
  
  - Pulling a KeyCloak docker image
  - Creating a client in KeyCloak for Oath2_proxy
  - Pulling a Oath2_proxy docker image
  - Setting up nginx as a reverse proxy

This is currently a work in progress and I am in the debugging stage, so please enjoy the Docker mascot in the meantime: 

![docker_Example]({{ site.baseurl }}/assets/images/docker_logo.png)


# Reflection
This internship has been an extremeley valuable experience for me because it has given me a glimpse into fullstack software engineering. Along with this, I was able to put into practice concepts I had learned from my classes such as designing databases and scrum methodology. It allowed me to enhance my skillset when it comes to translating business needs to technical specifications. No matter the direction my career takes, I am confident the knowledge and skills I’ve gained will be applicable. I am grateful to my team, Nevada Career Studio, and Address Income for making this a wonderful experience.
