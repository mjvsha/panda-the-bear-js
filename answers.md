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
