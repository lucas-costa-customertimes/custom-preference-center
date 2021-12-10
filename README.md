# Salesforce Marketing Cloud Custom Preference Center
A Starting Point for a Custom Preference Center for Salesforce Marketing Cloud

## Pre-Requisites
In order to use this project, you **must** be familiar with the following aspects of Salesforce Marketing Cloud (SFMC) and technologies:

### Required Knowledge

- CloudPages
- Server Side Javascript (SSJS)
- AMPScript
- Javascript
- HTML
- CSS

## Not required, but Nice to have knowledge:
- NodeJS
- Git or any other version control management system
- Basic programming skills: Functions, Loops
- Basic Understanding of Web Development concepts: GET and POSt requests

## The Custom Preference Center

This Custom preference center is **basic** and only saves data into Data Extensions. It does NOT save data into Salesforce CRM (but can be extended to do so).

You can access a sample of the Custom Preference Center here:

It contains the following main features:

1. Mobile responsive preferences form
2. Ability to control what options display on the preference center via Data Extensions
3. Tracking History feature that keeps track of every change made in the preferences by every subscriber (Can be good for Audit or debugging/reporting purposes)

# How to Deploy the Preference Center to a new Account
Follow the below instructions to deploy this repository to a Marketing Cloud Account. 

## Account pre-Requisites:
- CloudPages with SSL enabled (while this will work with CloudPages without SSL, it is not recommended)

## The Folder Structure

### /function-library/library.ssjs
File that contains all the functions that are used in the Custom Preference Center. This file must be loaded on top of **every page** of the Custom Preference Center.

> Failure to Load this file will result in the Custom Preference Center not working, and will result in a 500 error.

## /cloud-pages/
Folder that contains all the pages of the Custom Preference Center, including HTML and CSS files.

## /data-extensions/
Folder that contains all the Data Extensions that are used in the Custom Preference Center. Use Deployment Manager to deploy these Data Extensions or create them by hand with the required fields and naming conventions.

## Deploying to a Marketing Cloud Business unit






