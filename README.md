# Frontend Mentor - Notifications page solution

This is a solution to the [Notifications page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/notifications-page-DqK5QAmKbC). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)



## Overview

### The challenge

Users should be able to:

- Distinguish between "unread" and "read" notifications
- Select "Mark all as read" to toggle the visual state of the unread notifications and set the number of unread messages to zero
- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Screenshot

![](./screenshot.jpg)

Desktop View
 
 Check the Screenshots Folder

Mobile View

  Check the Screenshots Folder





### Links

- Solution URL: (http://boladaleakinpelufmc.io/)
- Live Site URL: (http://boladaleakinpelufmc.io/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- TailwindCss
- Flexbox
- Desktop-first workflow


### What I learned

What I learned(workflow) - I would like to try a mobile-first workflow, becasue I noticed whe I am done with the desktop version, I'd get very annoyed because the mobile version would be quite buggy. So I will try a mobile first approach to solve that issue. 

```html
<div class="img p-2 flex-none">
              <img src="/assets/images/avatar-kimberly-smith.webp" alt="" class="w-10 h-10 mx-auto">
            </div>
```
What I learned(html) - I learnt the flex-none utitility class to help keep the size and shape from shrinking or growing as the viewport shrank and grew. making the responsiveness feel more cohesive.

```js
<script>
    var toggleBtn = document.getElementById('togglebtn');
    var notificationCount = document.getElementById('notification-count');
    var text = "0";

    var notificationInst1 = document.getElementById("instance1");
    var notificationInst2 = document.getElementById("instance2");
    var notificationInst3 = document.getElementById("instance3");

    var subject1 =  document.getElementById("subject1");
    var subject2 =  document.getElementById("subject2");
    var subject3 =  document.getElementById("subject3");

    function toggleFunction() {
      notificationCount.textContent = text;

      notificationInst1.style.backgroundColor = "white";
      notificationInst2.style.backgroundColor = "white";
      notificationInst3.style.backgroundColor = "white";

      if ((subject1.classList.contains("after:text-red-500")) && (subject2.classList.contains("after:text-red-500")) && (subject3.classList.contains("after:text-red-500"))) {
        subject1.classList.add("after:invisible");
        subject2.classList.add("after:invisible");
        subject3.classList.add("after:invisible");   
      }
      
    }
  </script>
```

What I learned(Javascript) - I learnt the contains function for the classList, but also realised I did not fully understand the use of 'querySelector'. Moving forward I will try and get a grasp of it.


### Continued development

	While I worked on this challenge, I noticed that there were some concepts of the DOM I did not understand in Javascript, the querySelector function for instance. Moving forward I am going to practice using those functions so I can learn them and develop my skills. Also found more understanding of the flexbox concept and would like to use it more in future projects because it seems very useful.

### Useful resources

- [General Web Dev Knowledge](https://www.W3schools.com) - This helped me clarify some concepts with HTML, CSS and Javascript. I really liked this webpage because it is very concise and clear when explaining concepts and will use it going forward.
- [CSS](css-tricks.com) - This helped me open my eyes to the use and impact of CSS on my webpage and helped greatly with the understanding of Flexbox.
- [Tailwind](https://tailwindcss.com/) - This helped me understand the tailwind utilities and made me knowledgeable of tailwind as a whole.

## Author

- Website - [Boladale Akinpelu](Work-in-Progress)
- Frontend Mentor - [@DaleAkinpelu](https://www.frontendmentor.io/profile/DaleAkinpelu)
- Twitter - [@DaleAkinpelu](https://www.twitter.com/DaleAkinpelu)


## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.

**Note: Delete this note and edit this section's content as necessary. If you completed this challenge by yourself, feel free to delete this section entirely.**
