document.querySelector('.profile-image');
profileImage.src="https://timedotcom.files.wordpress.com/2015/04/snoop-dogg.jpg?quality=85"
 
Use the same approach to select the element that contains the photo of the sky and change the src attribute to another picture URL of your choosing.
var leftImage= Document.querySelector('#left-image img')
leftImage.src = 'https://i.ytimg.com/vi/OMaCBns4HMA/maxresdefault.jpg'
 
Select the heading that says "Panda the Bear" and change it to your own name.
var heading = document.querySelector('h1.highlight')
heading.innerText = 'Snoop the Lion'
 
Select the heading that says "Employment" and change it to something else. (hint: use a descendant selector)
 
var employment = document.querySelector('#employment  h3 ')
employment.innerText = 'SOME BULLSHIT!!'
 
Change the colour of the body.

var body = document.querySelector('body')

body.style.color= "red"

 
Change the colour of each element using the highlight class. Use a for loop to do this.
var highlight = document.querySelectorAll('.highlight')
highlight.forEach(function(h){h.style.color= 'orange'})
 
Change the font family of the h1 to 'monospace'.
var heading = document.querySelector('h1.heading')
heading.style.fontFamily= 'monospace'
 
Find a way to select the round icons in the sidebar and then change their colour.
var roundIcons = document.querySelectorAll('.action-icon-bg')
roundIcons.forEach(function(icon){
Icon.style.backgroundColor='yellow'})
 
 
Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself".

var form = document.querySelector('form.contact-info')
form.placeholder = 'identify yourself'

Change the placeholder attribute of the message field to "state your business".

 
var message = document.querySelector('#message')
message.placeholder = 'state ur bidness'
 
Give the name field a "value" attribute of "your nemesis".
form.value = 'your uncle'
 
Change the value attribute of the email field to "koalathebear@gmail.com".

var email = document.querySelector('#email')
email.value= 'koala'




Panda the Bear is lying about their skills! Take the "time travel" skill off the page to satisfy your personal sense of justice. Use your googling and docs-skimming skillz to find a jQuery function that will allow you to remove elements from the DOM. (hint: there are multiple ways of doing this, but the parent() function might be useful when it comes to selecting the right element)


var timeTravel = document.getElementById('time-travel');
var divBar = document.getElementsByClassName('bar-default')[2];

divBar.removeChild(timeTravel);


That drawing of Pikachu is really cute. Let’s duplicate it using cloneNode() and insert it at the bottom of the .portfolio-container using insertAdjacentHTML() or appendChild().

var pikachu = document.querySelector('#right-image img');
var pikachuClone = pikachu.CloneNode();
var portfoilioContainer= document.querySelector('.portfolio-container');

portfolioContainer.appendChild(pikachuClone);

Wow, that was so satisfying I think we should do it 10 more times. Use a for loop to help you do this.

for (var i = 0; i<10; i++) { var pikachuCloneTwo = pikachu.cloneNode(); porfolioContainer.appendChild(pikachuCloneTwo);
}

Let’s add a message about when the page was last updated. We'll do this by appending a new <li> element to the <ul> in the sidebar (you might need to refresh the page to bring back the list items that we emptied out earlier).

var listItem = document.createElement('li');
var leftSpan = document.createElement('span');
var textNode = document.createTextNode('Page Last Updated')

leftSpan.appendChild(textNode);
listItem.appendChild(leftSpan);

var bioInfo = document.querySelector('.bio-info');
bioInfo.appendChild(listItem);

var rightSpan = document.createElement('span');
var rightText= document.createTextNode('Thursday November 23rd 2017');
rightSpan.appendChild(rightText);

listItem.className = 'bio-info-item'
listItem.appendChild(rightSpan)
