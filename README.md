# Portfolio Project 
This is my portfolio Website

Github Repo:
https://github.com/aidanlawson31/Portfolio_website

Deployed Site:
http://amlawson.com/


# Documentation 

The purpose of my portfolio website, is to show the tools that I use and the projects that I am working on so that potential
recruiters have an idea as to who I am and what I do.

The features include: 
>A navbar, a landing page or homescreen, a skills and tools section, a project section, and a contact footer.
Some functionality:
>The navbar items highlight, and have a small animation when hovered over.

>When any link to a part of the site is clicked, a smooth scroll effect gives a good clean feeling when using the site, 
>this is made with one simple line of code under HTML in the scss file "scroll-behaviour: smooth;".

>A small moving arrow on the home page, when hovered over, moves down slightly to show the user that there is functionality
>here.

>in the projects section, screenshots of my Weebly projects are shown as "cards" with a hover effect.

# Design process

Trello.
When building my project, although I found Trello a useful tool for organisation and prioritization, I found it easy to forget to update my Trello
board on occasion. I did by best, even when forgeting, to go back and update it, as it helped me visualize my project. 
![trello](https://github.com/aidanlawson31/Portfolio_website/blob/master/Screenshots%20for%20project/Screen%20Shot%202019-05-18%20at%208.09.25%20pm.png)

When initially searching for inspiration, I looked through online blogs with titles similar to "Best Developer Portfolios".
A couple of the portfolios I really liked, and took inspiration from are: Yevgeniy Brikman — ybrikman.com, and Sean Halpin - seanhalpin.io.
These websites had a brochure style set up, minimalist design, and good colour coordination. All of these aspects were taken
into account when I was designing my website.

When designing my wireframes I used Figma.
I love Figma because I find it easier to use than balsamiq, it's 100% free with no subcribtion offer, AND it gives you the CSS code for more accurate dimensions.
My first design:
My first design used an image as the background, with minimalistic black styling, and white borders around elements.
![first-design](https://github.com/aidanlawson31/Portfolio_website/blob/master/Screenshots%20for%20project/Screen%20Shot%202019-05-15%20at%201.33.41%20pm.png)
However apon completing the first two sections, the home page and about section, I felt like the design wasn't quite where I had imagined it to be.
I liked the styling, but I decided against using an image as the background, instead opting to use colours, borders and shapes instead.

When designing my second wireframe I went back to my initial inpiration, this time following design, colouring, and features more closely.
![re-design](https://github.com/aidanlawson31/Portfolio_website/blob/master/Screenshots%20for%20project/Screen%20Shot%202019-05-23%20at%209.50.53%20am.png)
As you can see, I have more elements, a coloured background, clickable links for ease of use, and a design that would be more expandable in the future. Plus I no longer am sticking with a single image, reused multiple times.

For the personal logo, I simply used my initials, AL followed by a full stop, adding some element of design. AL. 

I created A timeline using Trello and Figma.
This timeline follows me through my re-design and gives an understanding about roughly what days were spent doing what.
![timeline](https://github.com/aidanlawson31/Portfolio_website/blob/master/Screenshots%20for%20project/timline.png)

# Site Components
>The NAVBAR.
Creating the navbar was relatively simple. The one interesting bit of code being:

  header::after {
    content: '';
    display: table;
    clear: both;
  }
  
This code is applied to the parent element, in this case the header. This clears the floats, fixing a bug where the nav bar elements were 
missaligned.

>The home page 
Again, is relatively simple, thanks to the minimal elements.
My favourite feature, maybe on the whole site is the floating arrow underneath the subtitle.
This was keyframes along with the CSS animation tool.

.about-arrow img {
  -webkit-animation: mover 1s infinite  alternate;
  animation: mover 1s infinite  alternate;
  display: block;
  margin-left: auto;
  margin-right: auto;
}

@-webkit-keyframes mover {
  0% { transform: translateY(0); }
  100% { transform: translateY(-10px); }
}

@keyframes mover {
  0% { transform: translateY(0); }
  100% { transform: translateY(-10px); }
}

Although I had to go to stack overflow to make this work properly, I edited the proportions, movement amount, and movement time, to fit the 
exact look I wanted to achieve.

>The about section.

The about section was a little tough, the header being my favourite part on this section. The header took some fiddling with and questions to get right. Originally I wasn't using flexbox, instead opting to hard code the header. Turns out the easiest way to do most things, and especially in this case with CSS is to use Flexbox. After fiddling with flexbox, using flex made the header responsive from the start.

>The skills and tools section.

This section was really quite hard for me.
For a long time I just could not get the icons to align the way I wanted them too. Eventually by editing the icons themselves outside of CSS, I was able to get them to be the same size, and use flexbox to align them neatly.

>The projects section.

I feel like the design in this section is lacking, however does get information across that I wanted.
Showcasing the Weebly screenshots as "cards" using a box shadow property:
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.6);
This give a much nicer effect than just posting the screenshots on the page.

# Documentation Questions
As part of the documentation we were tasked to answer 3 short questions:
1.  >Describe key events in the development of the internet from the 1980s to today (max. 150 words)
2.  >Define and describe the relationship between fundamental aspects of the internet such as: domains, web servers, DNS, and web browsers (max. 150 words)
3.  >Reflect on one aspect of the development of internet technologies and how it has contributed to the world today (max. 150 words)

# 1A.

In 1982 The first internet connection was made By a man named Kilnam Chon. The connection was later named SDN.
Kilnam Chon is a Japanese-born South Korean computer scientist. 

In 1988, the first internet exchange point, was established by connecting TCP/IP networks. 

In 1988 Daniel Karrenberg, a German computer scientist, created the first Internet Service Provider.

in 1989 the World Wide Web was created by Tim Berners-Lee, an English computer scientist.

And in 1991 The WWW was made available to the public.

In 1994 The first website was created, interestingly enough, for the Whitehouse.

Around 1994-1995 browsers as we know them, like Internet explorer, owned by Microsoft, as well as Netscape, owned by Verizon, and many other competitors were released.

in 2008 Google’s index of the web consists of one-trillion unique URLs.

Summer 2014 The number of Internet users worldwide reaches 3 billion.

# 2A.
HTTP stands for Hypertext Transfer Protocol, since 1990 HTTP has been used to enable communication, between "servers", and "clients". 

A Web Server can be software or hardware, that's purpose is dedicated to running, or hosting websites. The server processes the HTTP requests.

An IP (Internet Protocol) address is a unique number that is assigned to each device on the internet. Everytime you enter a website you need the IP that belongs to the web server that is hosting the webpage.

A DNS (Domain Name System) name allows us to call a webpage by a name, rather than an IP Address.

So a client, or web browser, makes a request to the server, via a URL, A DNS finds the associated IP Adress, sends the request
for a webpage the server, and then the server returns a response, in the form of a webpage. 

# 3A.

To me, the availability of medical help, mental or physical through online articles, chat rooms, and online doctors, has contributed positively
to the world. By allowing people who live in countries without free healthcare, who would otherwise not be able to help themselves, to get 
that help that they need. This is huge, for the youth and elderly especially. 
