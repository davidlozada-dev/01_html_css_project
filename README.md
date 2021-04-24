# 01_html_css_project

__Project's status: *finished*__ :heavy_check_mark:

## Index

1. [Introduction](#1-Introduction)
	
	1.[Motivation behind the project](#11-Motivation-behind-the-project)

	2.[Landing page layouts](#12-Landing-page-layouts)

1. [Technical aspects](#2-Technical-aspects)

	1.[Dropdown menu](#21-Dropdown-menu)

1. [Contributor](#3-Contributor)

## 1 Introduction

### 1.1 Motivation behind the project

This project is a fast way to put into practice fandamental HTML and CSS concepts by making a responsive landing page for a gameing store. 

#### Technologies/tools used for this project
	
	1. CSS
	2. HTML
	3. JavaScript

### 1.2 Landing page layouts

#### Desktop view

The __desktop view__ is composed by three parts; firstly, the header which holds four buttons on the top-right side and a nintendo logo on the top-left side. Secondly, the middle part shows a game controller and "add to car" butoon on the right side, while a brief description of the product and a animated button is shown on the left side. Finally, the footer which holds social media icons.

![Desktop view](https://raw.githubusercontent.com/davidlozada-dev/01_html_css_project/master/assets/img/desktop_view.png)

#### Mobile View

The __mobile view__ manages the same parts as the desktop view with the difference that the header doesn't hold the four buttons shown on the top-right desktop view. Instead, it holds a dropdown menu button and when it's clicked on it displays the four options as in the desktop view. 
	
![Mobile view](https://raw.githubusercontent.com/davidlozada-dev/01_html_css_project/master/assets/img/mobile_view.png)

## 2 Technical aspects

### 2.1 Dropdown menu

The dropdown menu is only shown on the mobile view, when the user clicks on the menu icon button activates a JavaScript function which compares the unordered list's maximum height whose default value is 0px on the mobile view and if it is 0px, it sets as new maximum heigh 130px displaying all four buttons showed on the desktop view as a list. Otherwise, if the unordered list's maximum height is greater than 0px, it sets as new maximum height 0px hidding all the four buttons.

```JAVASCRIPT

let menuList = document.getElementById("menuList");

menuList.style.maxHeight = "0px";

function togglemenu(){
	if (menuList.style.maxHeight == "0px") {
		menuList.style.maxHeight = "130px";
	}else {
		menuList.style.maxHeight = "0px";
	}
}

```

## 3 Contributor

Copyright © 2021 __David Lozada__