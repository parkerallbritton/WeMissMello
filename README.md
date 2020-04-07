Group Project - README Template
===

# Most Wanted App

## Table of Contents
1. [Overview](#Overview)
1. [Product Spec](#Product-Spec)
1. [Wireframes](#Wireframes)
2. [Schema](#Schema)

## Overview
### Description
An app for users to look up the most wanted criminals in the US.

### App Evaluation
- **Category:** Security
- **Mobile:** This app will be used on mobile devices, for simplicity's sake.
- **Story:** Display most wanted fugitive's from the official FBI list and give the option to search for a name in the list. 
- **Market:** Anyone from the large commuinity of those interested in crime/ crime shows could indulge, and read up on the official most wanted criminals.
- **Habit:** Purely for trivial and social purposes, not for the encouragement of anyone to attempt to hunt down individuals from the FBI's Most Wanted list.
- **Scope:** First, we will develop the app just for general display and search and then we could divide into different categories of crimes.

## Product Spec

### 1. User Stories (Required and Optional)

**Required Must-have Stories**

* User can see most-wanted list
* User can choose specific categories of most-wanted individuals, filtering the usual stream down
* User can tap on the photo shown of an individual and be taken to a detail screen

### 2. Screen Archetypes

* Stream
   * User can view a basic most-wanted list

* Categories
   * User can choose from an array of categories, filtering the usual stream down to gender, location, type of crime, age, etc. 

* Detail
   * Tapping on an individual's picture pushes the user to a detail screen, providing a detailed description of this person's criminal profile
   
### 3. Navigation

**Tab Navigation** (Tab to Screen)

* Home (stream)
* Categories
* Detail

**Flow Navigation** (Screen to Screen)

* Both categories and detail provide the option of navigating to the detail screen
   * Home => Detail
   
   * OR
   * Categories => Detail

## Wireframes
<img src="WireframeMWA.jpg" width=600>

### [BONUS] Digital Wireframes & Mockups
.
### [BONUS] Interactive Prototype

## Schema 

### Models
#### Main page
   | Property      | Type     | Description |
   | ------------- | -------- | ------------|
   | image         | String(URL)   | image of the fugitive|
   | title         | String   | name of the fugitive |
   | description         | String   | short summary of crimes |
   
#### Detail page   
   | Property      | Type     | Description |
   | ------------- | -------- | ------------|
   | image         | String(URL)   | image of the fugitive|
   | title         | String   | name of the fugitive |
   | description         | String   | short summary of crimes || dates_of_birth_used   | String   | DOB claimed by fugitive |
   |place_of_birth       | String  | birthplace of the fugitive  |
   |hair | String | fugitive's hair color |
   |eyes | String | fugitive's eye color |
   |height_min|Number|bottom end of fugitive's possible height|
   |height_max|Number|top end of fugitive's possible height|
   |weight_min|Number|bottom end of fugitive's possible weight|
   |weight_max|Number|top end of fugitive's possible weight|
   |sex|String|fugitive's biological sex|
   |race|String|fugitive’s race/skin color|
   |occupation|String|fugitive’s last known line of work|
   |nationality|String|fugitive’s country of origin|
   |scars_and_marks|String|identifying scars and marks on the fugitive’s person
   |person_classification|String|category of person’s involvement
   |warning_message|String|bolded text in description, “armed and dangerous”, etc.
   |reward_max|Number|financial compensation for information regarding fugitive|
   
 

  
### Networking
- [Add list of network requests by screen ]
- [Create basic snippets for each Parse network request]
- Base URL: https://api.fbi.gov/wanted/v1/list

