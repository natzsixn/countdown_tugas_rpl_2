# Keterangan

ini adalah tugas yang saya buat pada **28/02/2024** dan tema dari tugas ini adalah comming soon website dan bertujuan untuk mengenal **DOM** untuk pemula javascript termasuk saya:D

## 	javascript
	//code untuk menghitung countdown
	 javascript const seconds = document.querySelector(".seconds .number"),
	 minutes = document.querySelector(".minutes .number"),
	 hours = document.querySelector(".hours .number"),
	 days = document.querySelector(".days .number");
	 let secValue = 11,
		 minValue = 2,
		 hourValue = 2,
		 dayValue = 40;
	const timeFunction = setInterval(
		() => { secValue--; 
			 if (secValue === 0) {
			 minValue--; secValue = 60; 
			 } if (minValue === 0) { 
			 hourValue--; minValue = 60; 
			 } if (hourValue === 0) { 
			 dayValue--; hourValue = 24;
			 } if (dayValue === 0) { 
			 clearInterval(timeFunction);
			 } 
	seconds.textContent = secValue < 10 ? `0${secValue}` : secValue; 
	minutes.textContent = minValue < 10 ? `0${minValue}` : minValue; 
	hours.textContent = hourValue < 10 ? `0${hourValue}` : hourValue; 
	days.textContent = dayValue < 10 ? `0${dayValue}` : dayValue; }, 1000); //1000ms = 1

	//code agar text ket lebaran tidak sangat panjang 
	//hanya setengah saja yang di tampilkan
	var  keteranganCarousels  =  document.querySelectorAll(".second");
	var  displayCharacters  =  120;
	keteranganCarousels.forEach(function (element) {
	var  originalText  =  element.textContent;

	var  trimmedText  =  originalText.slice(0, displayCharacters);
	var  displayText  = trimmedText  + (originalText.length  >  displayCharacters  ?  "..."  :  "");

	element.textContent  =  displayText;
	});
	
## code html yang tersambung ke js
All your files and folders are presented as a tree in the file explorer. You can switch from one to another by clicking a file in the tree.

## Rename a file
berikut code untuk countdown class number  di wrapper time:
```
<div  class="countdown">
	<div  class="time days">
		<span  class="number"></span>
		<span  class="text">days</span>
	</div>
	<div  class="time hours">
		<span  class="number"></span>
		<span  class="text">hours</span>
	</div>
	<div  class="time minutes">
		<span  class="number"></span>
		<span  class="text">minutes</span>
	</div>
	<div  class="time seconds">
		<span  class="number"></span>
		<span  class="text">seconds</span>
	</div>
</div>
```

ini code untuk ellipse text agar ga kepanjangan:

```
var  keteranganCarousels  =  document.querySelectorAll(".second");

  

var  displayCharacters  =  120;

  

keteranganCarousels.forEach(function (element) {

var  originalText  =  element.textContent;

  

var  trimmedText  =  originalText.slice(0, displayCharacters);

var  displayText  =

trimmedText  + (originalText.length  >  displayCharacters  ?  "..."  :  "");

  

// Update the text content of the element

element.textContent  =  displayText;

});
```

## penutup

suwun yang udah follow githubku:D
