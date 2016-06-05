##How to make an element flip with CSS and Jquery.

Start by creating a div give it a cool class name. I suggest "card" or "thingIWannaFlippyFlip". But you can make it what ever you like. Hop on over to your CSS page. Now give it a height and a width and a nice background color. I prefer black. Like my soul. Now refresh the page and behold your beautiful Frankensteinian creation. Not showing up? Make sure you link that stylesheet up to that HTML guys!

Awesome. Now it's to make that mamajama flip. CSS again. take your div and tell it what we want it to do. Transition: transform then an amount of time you want it to take. Want it to slow roll like Snorelax after some cough syrup? Then try this-

.card {
  transition: transform 15s;
}
Want it to flip as quick as a spider monkey hopped up on Mountain Dew? Try this...

.card {
  transition: transform .25s;
}

Awesome. Refresh and click on that div and WATCH WHAT HAPPENS!!!

nothing...don't cry sweet front end warrior. We ain't done yet. Now we gotta make a new class for our little card. "flipped" is a good name. Now in that bad bad boy we telling it how we want to transform it. Poor us though...css doesn't understand what flip means, silly css so try this...

.flipped {
  transform: rotateY(180deg);
}

AWESOME! Refresh and see what happens? NOTHING AGAIN! MY COMPUTER IS BROKE I DIDNT SAVE IT WHATTTTTTTTT.
Nope. Its all ok still not done.

Time to hop on over to our friend Jquery. Now when we click this div we want it to flip. How we do that? Try this?

$(div).click(function {
  $(this).addClass("flipped")
  });

Now refresh...wait...your computer is 4 years old its slow...wait...CLICK! and?? and??

YOU ARE A PROGRAMMING GOD! 
