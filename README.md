# csportfolio

Hey

Here's my comp sci portfolio


Here's a link to my HTML/CSS [site](https://gertonsonc.github.io/testWeb/dogPage/index)

Here's my [lightning project](https://gertonsonc.github.io/lightning2/)

Here's my [Dice Program](https://gertonsonc.github.io/dice/)

Here's my [Chemotaxis](https://gertonsonc.github.io/chemotaxis4/)

This is some of the hardest code I've written this year. This is from **Chemotaxis**

'''Java
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

'''
