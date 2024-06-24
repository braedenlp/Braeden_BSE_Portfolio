# LED Matrix Scoreboard
If you have ever played a basketball game at an arcade, this project is a perfect desktop version. I built an interative basketball hoop that will count your score every time you make a basket, it will then display your score on the backboard. The way this works is that there are sensors in the hoop that detect when a ball goes in, it then relays that information to the circuit which then makes the score go up.






| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Braeden P | Sacred Heart Prep | Electrical Engineering | Rising Sophmore

<!--**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**-->

<iframe src="https://drive.google.com/file/d/1Qb_cBo46hmILoujQ7SBQeim7MhqIJjBN/preview" width="640" height="480" allow="autoplay"></iframe>
  
# Final Milestone

<iframe width="560" height="315" src="https://www.youtube.com/embed/GilUcbJHTUQ?si=prKn_NBWJCFLiVs2" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE


# Second Milestone

<iframe width="560" height="315" src="https://www.youtube.com/embed/UzoG46Dgx08?si=HmRxoATlQNrEgput" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Summary
Since my first milestone, I have worked on the software aspect of my project. There was a sample code that the developers of the project provided that I used, but some of the code didn’t work. I have been troubleshooting their code and I have made it functional, but there are some aspects that I want to change. For example, I need to change the delay so that the project will properly count the score. The purpose of the delay in this specific project is not to overload the feather with too much input from the sensor. It also controls the sensitivity of the sensor because while the delay is happening, the code isn’t running. So any input that the sensor receives while the code is stopped the feather will ignore. When I put the delay very low, for instance at 0.01, the score would start auto counting and go up eight with just one basket. This would happen because the delay in the code was less than the time it took for the ball to pass through the hoop. But when I put the delay higher, it wouldn’t detect the ball some of the time. This would happen because if the delay is high, the program does a lot of waiting. The state of the sensor isn’t constantly being checked, so if I were to make a basket in that state of waiting, it wouldn’t sense the ball go through. So I have to troubleshoot to find the perfect median between sensitive and not. 

![diagram](Blank diagram (1).png)

Figure 1: The figure above is a finite state machine of my code.

## Challenges

This milestone has been challenging especially since my computer didn’t work with the software halfway through the process. For instance, it would keep giving me error codes saying that it couldn’t read information in a number of the files even though my computer worked perfectly with the files earlier in the process. The other problem I had which was my wires kept snapping still has been a problem throughout this problem. The project is at a point where every wire is either tinned or has a more sturdy solid core wire soldered onto it.

## Next Steps

I hope to finish troubleshooting my code by the end of the week so I can start working on modifications.

# First Milestone

<iframe width="560" height="315" src="https://www.youtube.com/embed/ktwYQZghSSA?si=WxeESJleusiH3-68" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## What My Project is

My project is a mini hoop with a scoreboard. It has sensors in the hoop that will detect when a ball goes through. The hoop will then make the score on the scoreboard go up by two just like basketball. It also has a button that starts a new game and resets the score. This milestone was mainly hardware, I put together the entire hoop and connected all the wires. I also soldered all of the parts together. Some things that I soldered were all the wires to the pins on the feather express and featherwing, and the wires connecting to the button. Every time a wire snapped I soldered a solid core wire onto the tip of it or I tinned it. There were also connectors that I soldered onto the featherwing and feather express so that the feather express could rest on top of the featherwing. 

![hardware](Untitled presentation (2).jpg)

Figure 2: The figure above is a picture of my project built and wired. The arrows point towards the most important parts of the project.
![schematic](led_matrices_circuit-diagram.jpg)

Figure 3: The figure above is a schematic of all the wiring that I did.

Figure Reference: Adafruit
## Challenges

The main challenge that I faced in building the hoop was the process of altering multiple mechanical aspects of my project for it to work. For instance, I used a dremel to sand down the acrylic covering of the matrix board because it was too big. I also had to reprint the legs of the hoop as they were too small. The biggest annoyance was that the wires kept snapping off of my circuit boards so I either soldered solid core wires onto them or tinned them. On top of all that, the matrix board that I have right now is broken so we have to get a new one. What came with this was a lot of debugging because I initially thought that something was wrong with my circuit board or my wiring. I ended up using a different, bigger, matrix board that was proven to work to hook everything up.

## Next Steps

The next step I want to take in my project is to get all of my software working. This is getting my sensors working, the button, and the speaker all to work. None of this is working right now and it is very frustrating so I hope to figure all of this out.

<!-- # Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

# Code
Here's where you'll put your code. The syntax below places it into a block of code. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize it to your project needs. 

```c++
void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  Serial.println("Hello World!");
}

void loop() {
  // put your main code here, to run repeatedly:

}
```

# Bill of Materials
Here's where you'll list the parts in your project. To add more rows, just copy and paste the example rows below.
Don't forget to place the link of where to buy each component inside the quotation marks in the corresponding row after href =. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize this to your project needs. 

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
-->
# Starter Project: Calculator
<iframe width="560" height="315" src="https://www.youtube.com/embed/Lc4bP4zvc5Q?si=o-6FkkPM0eynmOZC" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

[Link to my Starter Project](https://www.amazon.com/Kit-Calculator-Resistance-Electronic-HUAGZIMO/dp/B0D13C9SYT/ref=sr_1_3?crid=3HGJTLNZ9O2GX&dib=eyJ2IjoiMSJ9._SWtzcdxglPoBR9j02Ru8HdkQYctYGhXoQSzf1MVwW8-wdJNSkQkLmCAtn4dRp6g-6R7J9461vhIP2EF_nk7Tig6XDG9bCrlMTSlmck5MBQwLRhhnSiQUGo0QJa1GwgSj6a6-1yBKFqneN2-Z0AqO-StnMGL2G8655x5qfsjKhjBt48dYiTRy3_0E2_Jk5agtyEMTLExRFtYVrPI5ML2CKLPh8c4dT4clp-o5in2kS0.ajrpXguZyLba8zZbq_b1WT_1ccEQlOe_PpesP9bkSUM&dib_tag=se&keywords=calculator+solder&qid=1717994208&sprefix=calculator+solde%2Caps%2C148&sr=8-3)

## Summary
I chose the calculator for my starter project because I wanted something that I will actually use and have an everyday use for. The way it works is that there is the integrated circuit, or IC, which performs all the calculations. The IC receives the input from the buttons when the buttons are pushed because the button closes a switch, which connects the circuit providing voltage to the IC. When the buttons are in their unpushed position, the switch is open so there is no current between the battery and the IC, but when the button is pushed, it closes the switch onto the circuit which connects a current with voltage to the IC. A switch is an electrical component that disrupts the current in a wire. The IC then displays the number then finished calculation on the seven segment display. The assembly process was pretty simple, the majority of the building process was soldering.
<img width="691" alt="Screenshot 2024-06-11 at 3 50 14 PM" src="https://github.com/braedenlp/Braeden_BSE_Portfolio/assets/172335639/1ac4e1e3-bdfa-4387-98d2-d1727618aba6">

Figure 4: The figure above shows how switches function on an electrical circuit. The left shows an open switch and the right shows a closed switch, so the left would be an unpushed button and the right would be a pushed button. The difference between the two is that the left is an open circuit and the right is a closed circuit which means that the right can provide current to the light to light it up while the left can not.

Figure Reference: Research Gate
## Components Used

- Monolithic Capacitor
- CR2032 Battery
- CR2032 Battery Socket
- Black-Yellow Button
- White Button Cap
- Transparent Button Cap
- Micro USB Socket
- 3Bit Digital Tube
- STC15W408AS Controller
- IC Socket
- Button Labels
- Acrylic Board
- M2*2*+3mm Copper Pillar Screw
- M2*20mm Screw
- M2*4mm Screw
- M2 Nut
- PCB Circuit Board

## Challenges

Some challenges I faced were soldering and putting the case on. Soldering was somewhat challenging due to the fact that the majority of the project was soldering and some parts were small which made it harder to be precise while keeping the project clean. Another challenge I faced was the case. In the beginning of putting the case on, the battery didn’t fully fit into the slot and the charger didn’t fit into the slot for the charger.

## Next Steps

I am very excited to start on my main project and to see what I can learn from it.

<!--# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)

To watch the BSE tutorial on how to create a portfolio, click here.-->
