---
layout: post
title: "CLAPP User Handbook"
date: 2021-04-08
categories:
  - documentation
tags:
  - documentation, handbook, CLAPP
---

# CLAPP - Customer Loyalty in a Small Package
![](https://rohitbassi.me/images/clapp.jpg)

> ## Table of Contents
> 
> - [Introduction](#intro)
> - [Getting Started](#get-started)
> - [Using CLAPP](#using-clapp) 
> - &nbsp; &nbsp; &nbsp; [Adding a New Customer](#add-customer)
> - &nbsp; &nbsp; &nbsp; [Finding a Customer](#find-customer)
> - [Additional Resources](#add-res)
> - [CLAPP for Developers](#clapp-supp)


### <a name="intro"> What is CLAPP? </a>

CLAPP is a customer loyalty program designed for small businesses. There are many kinds of software out there that have options for customer loyalty data storage, however most of those applications are subscription based or require upfront purchases. CLAPP is a customer data management program that is lightweight and open source, allowing it to run on low-spec Windows based POS systems. Since it is open source, experienced developers also have the ability to make changes to the code to fit the exact specifications of a users requirements. In this handbook, I will be covering how to download, run, and operate CLAPP on a Microsoft Windows environment.

### <a name="get-started"> Getting Started </a>

First, click [**here**](https://github.com/r-bassi/CLAPP) to open my GitHub repository containing the files you will need to download. Navigate to and click on the green code button, and then click on download ZIP:
![](https://rohitbassi.me/images/clappdownload.png)

Once you have downloaded the ZIP file, navigate to where you have saved the file and right click -> extract the ZIP file to the given folder using an unzipping tool of your choosing (WinRAR, 7zip, etc.):
![](https://rohitbassi.me/images/extract.JPG)

Open the newly extracted folder, where you will find **CLAPP.jar**:
![](https://rohitbassi.me/images/clappjar.JPG)

Double click on **CLAPP.jar**, and you will see the main screen for the CLAPP application. Now you are ready to begin storing, updating, and searching for  customer information.

### <a name="using-clapp"> Using CLAPP </a>

Once you have opened up CLAPP, you will see the options to add a new customer, find a customer by their recorded name, find a customer by their customer number, and add to a returning customers total spending. The blank white area at the bottom of the application is a log of the past few actions within the application, which can be cleared using the clear button. 

<a name="add-customer"></a>
To add a new customer, simply click on the "New Customer" tab and enter the customers information, along with the amount they have spent at their current visit, and click "Submit":
![](https://rohitbassi.me/images/clappgood.JPG)
&nbsp;


<a name="find-customer"></a>
Once you add a new customer, you may find a customer by their name or number. Searching for a customer by their name is case and character sensitive, so to find a customer that has been added, we must search for their exact name as was stored in the New Customer tab: 
![](https://rohitbassi.me/images/findnum.JPG)

The other option is to find them by the customer number that you assigned to them:
![](https://rohitbassi.me/images/findnum2.JPG)


### <a name="add-res">Additional Resources</a>

I hope to have helped you with using CLAPP with this post. If you require more assistance with setting up Java or JDK dependencies, take a look at these articles [here](https://www.java.com/en/download/help/index_installing.html) and [here](https://docs.oracle.com/javase/8/docs/technotes/guides/install/windows_jdk_install.html). If you are having any problems with CLAPP, feel free to [send me an email](mailto:rohit.bassi@outlook.com) and I will try to help you as much as possible. Feel free to share this post using the links at the top or bottom of this page, or anywhere else.

### <a name="clapp-supp"> CLAPP for Developers </a>

Currently, the only developer involved with CLAPP is [me](https://rohitbassi.me/). If you would like to improve upon CLAPP, feel free to fork the repository and experiment at will. 

Some things that have not yet been implemented are listed in the README.md of the CLAPP application, and on the CLAPP GitHub page [here](https://github.com/r-bassi/CLAPP).