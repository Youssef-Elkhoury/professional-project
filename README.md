## welcome to my new profile website

## my profile website is mainly divided of 3 sections

1. index.html (which is my main profile home page)
2. gallery.html (which is my photo gallery page)
3. contact.html (which is where to contact me page)

## I created css file for every page and linked them.

## In index.html file i add the following:

1. In the header i created a Navigation bar with logo using the following code:
<header>
        <img src="./img/index/portlogo.png" alt="port logo" />
        <nav>
            <ul>
             <li>
             <a href="./index.html">Profile</a>
             </li>
             <li>
             <a href="./gallery.html">Gallery</a>
             </li>
             <li>
             <a href="./contact.html">Contact</a>
             </li>
            </ul>
        </nav>
</header>

2. In the body i add my profile photo and information about me and i add icons to my information using the following website:
   (https://fontawesome.com/)

3. I add hover effect to my navigation bar using the following code add in my index.css file:

nav a:hover {
background-color: goldenrod;
color: black;
}

@keyframes slideFromRight {
0% {
transform: translate(20%);
}
50% {
transform: translate(-200%);
}
}

4. I add the following code to my index.css file to let the navigation bar sticked 100% on the top of my page with no blanks:

html {
scroll-padding-top: 100px;
}

## In image.html file i added the following :

1. add photo gallery using the following code:

<section id="gallery">
           <div>
              <img src="./img/gallery/server.jpg" alt="server room photo" />
              <img src="./img/gallery/server1.jpg" alt="server room photo1" />
              <img src="./img/gallery/server2.jpg" alt="server room photo2" />
           </div>
           <div>
            <img src="./img//gallery/server3.jpg" alt="server room photo3" />
            <div class="placeHolderDiv"></div>
            <img src="./img/gallery/hardware1.jpg" alt="Hardware photo1" />
           </div>
           <div>
            <img src="./img/gallery/hardware2.jpg" alt="Hardware photo2" />
            <img src="./img/gallery/hardware3.jpg" alt="Hardware photo3" />
            <img src="./img/gallery/coding.jpg" alt="coding photo" />
           </div>
      </section>

2. I give it animation effect using the following code in images.css file:

@keyframes pop {
0% {
transform: scale(1) rotate(0deg);
}

    50% {
        transform: scale(0.8) rotate(-180deg);
    }

    100% {
        transform: scale(1.2) rotate(360deg);
    }

}

#gallery img:hover {
animation: pop 0.5s forwards;
box-shadow: 5px 5px 5px goldenrod;
}

## In contact.html file i added the following :

## I create a section with 2 divisions 1st for social media and 2nd for contacting form by using the following code:

1. social media code:
   <div>
   <article>
   <h2><i class="fa-solid fa-earth-americas fa-2xl" style="color: #ffffff;"></i> Social Media</h2>
   <p><i class="fa-brands fa-facebook fa-lg" style="color: white"></i> Facebook</p>
   <p><i class="fa-brands fa-square-twitter fa-lg" style="color: white;"></i> Twitter</p>
   <p><i class="fa-brands fa-instagram fa-lg" style="color: white;"></i> Instagram</p>
   <p><i class="fa-brands fa-linkedin fa-lg" style="color: white;"></i> Linkedin</p>
   <p><i class="fa-brands fa-discord fa-lg" style="color: white;"></i> Discord</p>
   </article>
   </div>

2. contact form code:
<form>
<div>
<label for="name">Name:</label>
<input type="text" id="name" name="name" required>
</div>
<div>
<label for="email">Email:</label>
<input type="email" id="email" name="email" required>
</div>
<div>
<label for="subject">Subject:</label>
<input type="text" id="subject" name="subject" required>
</div>
<div>
<label for="message">Message:</label>
<textarea type="message" name="message" rows="5" cols="30" required></textarea>  
 </div>
<div>
<input type="submit" value="Send Message">
</div>
</form>

<!-- action="submit.php" method="POST" to add after form as id to activate submit later-->
