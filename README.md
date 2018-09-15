# Bicycle Vest
A bicycle safety vest with LED turn signals. I'm writing this guide as I go and I'm not nearly done, so the guide isn't nearly done!

## Background
I'm on a physical computing kick. I built a bunch of Arduino projects and then stretched my knowledge with an Internet of Things project (my [beer temp sensor](https://github.com/craftykate/beer-temp) that takes the temp of fermenting beer, uploads the temperature data online and sends texts if the temp goes too high or too low) and then I wanted to stretch a little more and do a wearable tech project...

## Problem to Solve
I love to ride my bike. My toddler loves to ride on the back of my bike with me. The drivers around town love to speed and run stop signs. I wanted something that would make us more visible and also alert drivers when I was going to be turning. This seemed like the perfect opportunity for a wearable project!

## The Solution
I'll fill this out once I finish the project and have all the details finalized =)

## Why Read This
I consider myself maybe an advanced beginner with microcontrollers. I learn a lot more with each project but there's still a lot I don't know. This is my first wearable tech project. Read this if you'd like to venture into wearable tech or if you're curious about programming a micro:bit or maybe you're trying to build an LED turn signal vest! I also try to keep my projects simple and cheap, which is good for beginners!

## Design Considerations
There are a lot of right ways to design this and I pondered a lot of them. 

I knew I wanted the LED turn signals to be on my body and chose a vest because it's often hot here and I knew a full jacket or sweater would be too much. I chose a basic white vest because I didn't want reflective tape on more traditional safety vests to distract from the LEDs. 

The triggers took more thought. Originally I wanted to put right and left turn buttons on the handle bars and send a bluetooth signal to the vest, and this would be a great solution, but as a study in wearable tech I ultimately wanted the whole thing to be wearable. I also wanted it to work anywhere, not just on that one bike. This would leave options open for additional features (maybe it can light up if I'm walking in the dark) and would allow me to bring it to the schools that I volunteer at and show them how the whole thing works without needing to drag my bike along, too. 

HOW to trigger the turn signals took more thought. I was stuck on buttons for a while but couldn't think of a good solution that didn't require taking my hands off the handle bars. Buttons on the ends of the sleeves would have been a pretty good solution, but like I said above, I didn't want sleeves. I took a few bike rides and thought about how I move my body and what kinds of sensors are available and what movements would be intuitive and easy and eventually realized that my head moves pretty freely - I could tilt my head to the left or right to trigger left or right turn signals. I looked into several different kinds of microcontrollers and sensors and one of the simplest solutions I could think of was already in my inventory - a [micro:bit](https://www.sparkfun.com/products/14336)! It's small, relatively cheap ($16.50), has bluetooth capabilities and has tilt sensors built in. It also has a 5x5 matrix of LEDs on the front for instant feedback. 

So I settled on a micro:bit on my helmet that senses if I tilt my head and that will trigger left or right turn signal LEDs on the back of my vest. I thought at first I'd send a bluetooth signal to a LilyPad on my vest but making a LilyPad bluetooth compatible looked like it was going to cost a lot more than just two micro:bits - one on the helmet and one on the vest. And THEN I realized there wasn't a whole lot of space between my helmet and the back of my vest so maybe two microcontrollers were overkill anyway and I could just connect the wires with a detachable connector. So that's my plan. Hard wire the whole thing. I got a connector that looks like it will be easy to connect and disconnect behind my head but if that changes I'll redesign. 

## Equipment
Working on this...
