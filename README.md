# Comp Sci Portfolio !!

Hey how's your day been?

<details><summary>HTML Site</summary>
SITE LINK:
https://gertonsonc.github.io/testWeb/dogPage/index
    
CODE: 
https://raw.githubusercontent.com/GertonsonC/testWeb/gh-pages/dogPage/index.html

  <details><summary>:arrow_right:Website Reflection:arrow_left:</summary>
    <p> This project was interesting for me. I have really only had expirence with Java, and it was interesting learning how different some other languages are. Making it about lil pump was also kinda fun just because of his meme status. Overall, this project taught me a lot about the implementation of HTML and CSS to allow a program to run effectively online.
    </p>
  </details>
</details>


<details><summary>Lightning</summary>
    THIS PROJECT DOES NOT WORK DUE TO THE LACK OF A REPOSITORY OOPS
    
PROJECT LINK:
https://gertonsonc.github.io/lightning2/
    
CODE:
https://raw.githubusercontent.com/GertonsonC/lightning2/gh-pages/Lightning.pde?token=AeS-YMI2yng9XZQcDzGw9e4lxIpy2FF1ks5cBefGwA%3D%3D
 
  
  <details><summary>:arrow_right:Lightning Reflection:arrow_left:</summary>
    <p>This project was one that I enjoyed making. Using the random() was cool to see how setting different parameters and changing them can have vastly different effects in the program. It was a good introduction back into Java after the summer. When I first made the lightning, I had the idea of making it sith lightning like in Star Wars, so I got Darth Sidious and the most iconic star wars song to accompany my program. This program was relatively easy to make but it was fun to do.
    </p>
  </details>
</details>


<details><summary>Dice</summary>
PROJECT LINK: 
https://gertonsonc.github.io/dice3/
    
CODE:https://raw.githubusercontent.com/GertonsonC/dice3/gh-pages/Dice.pde?token=AHSL4YG3GMPRJXYZXOU6HM2462ZFC

  
  <details><summary>:arrow_right:Dice Reflection:arrow_left:</summary>
    <p>
   Dice really took me a while to make. It was hard for me to come up with an idea that would stand out. In fact, my original idea had the dice spinning on their own and you could click the mose to stop and take a pause in the program, and click again to resume it. I used the delay() method in processing which doesn't seem to work in the web browser, so I made the dice rolling manual. One thing that I did that was cool was using only RGB values above 150 to make the pastel colors of the dice contrast with the darker background.
    </p>
  </details>
</details>


<details><summary>Chemotaxis</summary>
PROJECT LINK: 
https://gertonsonc.github.io/chemotaxis4/ **DOES NOT WORK ONLINE**
    
CODE:https://raw.githubusercontent.com/GertonsonC/chemotaxis4/gh-pages/Chemotaxis.pde?token=AHSL4YCIHNY7HHUH5MJQSJK462YO4


<details><summary>:arrow_right:Chemotaxis Reflection:arrow_left:</summary>
    <p>
  This was the program that took me the longest to make. When the project was first introduced, I knew I wanted to make it into a game. I had so many if statements that would always be checking if things were true that could slow down the particles, end the game, or move the particles. This took me a while to make just to get everything working with no issues. Using arrays to constantly track the X and Y coordinates of the particles took a while to set up, and getting the hitboxes of the particles just right took me a while just itself. I really like how this project turned out, but unfortunately it doesn't work online due to the delay() function being used, and it's the whole backbone of my program so I couldn't just take it out.
    </p>
  </details>
</details>


<details><summary>Starfield</summary>
PROJECT LINK: 
https://gertonsonc.github.io/starfield5/
    
CODE:https://raw.githubusercontent.com/GertonsonC/starfield5/gh-pages/Starfield.pde?token=AHSL4YCOTD6TXMF5U76N232462YVG


<details><summary>:arrow_right:Starfield Reflection:arrow_left:</summary>
    <p>
  The hardest part of starfield for me was getting the particles that bounce off the walls to work. It took me forever just to figure out how I would be able to move all of them at once and track their X and Y values so I could reverse them if necessary when hitting a wall. I added in the reverse when the mouse is pressed thing last second to make my program less generic, but it led to a cool bug that I left in that makes the spinning particles look different. This one was very frustuating to make, but the end result was pretty cool.
    </p>
  </details>
</details>


<details><summary>:arrow_right:Additional Reflections:arrow_left:</summary>

<p>
    One thing that I was proud of was my chemotaxis in general. I came in before school like every day to get this done, and finishing it was really hard. I had to make sure all the hitboxes work, I had to constantly be checking the X and Y positions of all the particles, check them for colission, and make them move at a reasonable scale. I had to add a working timer that stopped after 60 seconds. I had to get everything to line up and look nice on the display, and there were so many other thigns that made this the hardest program for me. I'm glad that I got through it and that I worked hard to come up with a final product that ended up woking really well and being cool. Nothing anyone else did was anything like it, and I thought that was cool. My code for this is above in the Chemotaxis section. It does not work on the web browser due to the use of the delay() method, but if you copy/paste it in Processing it should work fine.
    </p>
    <p>
    Another thing I am proud of is how I learned all this stuff about HTML and CSS. 3 months ago if you asked me what CSS was, I would've had no idea. Now with all the work I put into my website, I know just how far you can go with HTML and CSS to make a website that not only looks nice, but has functionality and can do cool things. One thing that was suprisingly easy was implementing youtube videos into the site, but that added to the whole thing overall. Learning all that was really fun and cool, and I want to learn other languages that aren't similar to Java for the same reason.
</p>

<p>
        The biggest hurdle for me to overcome was for me to get my bouncing particles to work in Starfield. I was just very confused at how you would use an interface to link everything together and I was focusing too much on that. What I eventually ended up doing was looking at the falling snowflakes from the christmas card last year and using that code as a foundation for those stars.
</p>
    
This is some of the hardest code I've written this year. This is from **Chemotaxis**

```
  void draw()   
{ 
  if (startT==false){
    background(128);
    text("Click to start",216,377);
  }
  if (startT==true)
  {
    int passedTime = millis() - sec;
    int col1 = (int)Math.floor(Math.random()*106+150);
    int col2 = (int)Math.floor(Math.random()*106+150);
    int col3 = (int)Math.floor(Math.random()*106+150);
    del = 10;
    background(0);
    background(128);
    noLoop();
    for (int i=0; i<=14; i++)
    {
      org.show(ox[i], oy[i], col1, col2, col3);
    }
    org.move();
    for (int i=0; i<=14; i++)
    {
      if (ox[i]==mouseX && oy[i]==mouseY) {
        textSize(60);
        text("YOU LOSE!", 249, 377);
        endL=true;
      }
    }
    textSize(40);
    fill(255);
    text(time,100,100);
    text(pCount, 700, 50);
    rect(700,75,25,100);
    fill(128);
    rect(700,75,25,100-pCount);
    fill(col1, col2, col3);
    if (mouseButton==LEFT && pCount>0) {
      pCount--;
      del = 70;
    }
    if (passedTime > total){
      time--;
      sec=millis();
    }
    if (time==0){
      endW=true;
      text("YOU WIN!",265,379);
    }
    if (endL==false && endW==false) {
      delay(del);
      loop();
    }
  }
}
```
</details>
