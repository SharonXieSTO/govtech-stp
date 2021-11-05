---
title: TestAccordian
permalink: /testaccordian
---

<html>

<head>
<meta charset="utf-8">
<title>CSS Accordion</title>

<style>

input {
    display: none;
}

label {
    display: block;    
    padding: 18px 50px;
    margin: 0 0 1px 0;
    cursor: pointer;
    background: #153855;
    border-radius: 3px;
    color: #FFF;
    transition: ease .5s;
	position: relative;
}

label:hover {
    background: #346f9e;
}

label::after {
	font-family: "Font Awesome 5 Free";
	content: '\271A';
	font-weight: bold;
	font-size: 22px;
	position: absolute;
	right: 10px;
	top: 6px;
}

input:checked + label::after {
	content: '\2212';
}

.content {
    background: #FFFFFF;
    padding: 10px 25px;
    margin: 0 0 1px 0;
    border-radius: 3px;
}

input + label + .content {
    display: none;
}

input:checked + label + .content {
    display: block;
}


</style>

</head>

<body>


<input type="checkbox" id="title1" />
<label for="title1">1. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</label>

<div class="content">
	<p>The following FAQs apply to persons who are residents in countries/regions that have established RGL arrangements with Singapore seeking single-entry, short-term essential business and official visit into Singapore:</p>
</div>

<input type="checkbox" id="title2" />
<label for="title2">Accordion Two</label>

<div class="content">
<p>Your content goes here.</p>
</div>

<input type="checkbox" id="title3" />
<label for="title3">Accordion Three</label>

<div class="content">
<p>Your content goes here.</p>
</div>
</body>




