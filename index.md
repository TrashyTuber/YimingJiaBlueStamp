# MIDI Controller
Imagine that you want a piano just for fun but realize that they cost thousands of dollar and there's no way you will spend that much. This project here contains all the basic components of a digital piano and even an LCD display showing the volume and instruments selected. 

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Yiming Jia | Dougherty Valley High School | Electrical Engineering | Incoming Sophomore

![Headstone Image](https://bluestampengineering.com/wp-content/uploads/2016/05/improve.jpg)
  
# Final Milestone

I was basically done with my controller at at the second milestone as I have already finished making the controller and its functions but I wanted to add a display showcasing the instruments so you can see what you have selected. The LCD part I got was an I2C so there was only four ports I needed to plug into and for the vcc part, I soldered my previous 5v wires up to a resistor and the new one to the end of it since I was having crashes from my potentiometers at max value. Once that was completed, I imported the library for LCD I2Cs and used it to output text when the value of the potentiometer for intruments changed. I also didn't know what to do for the second line of the LCD so I added a volume bar and I was able to test out special characters using hexcode for it. I did basically the same thing for what I did for the instruments and checked if the value for it has changed. In the end, my product can produce notes, switch octaves, adjust volume and instruments and have it show up on a display, and other smaller things like the reverb settings and a sustain pedal. 

<iframe width="800" height="450" src="https://www.youtube.com/embed/stWiOH5JV6s" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

# Second Milestone

My second milestone was mainly making the box of the controller and soldering all the wires that connect the buttons to the arduino board. For the box, I didn't have the right tools to cut the circles for my buttons so I just used a compass to map it out and a small scissor to cut it. For the potentiometers and the sliders, the holes were to small to use a compass so I drew the point out and use a pencil to shove a hole out until it's big enough for the potentiometer to fit in. The soldering took a long time for me to get used to but I basically used one type of wire to connect up all the 5v and another for the ground. The other port of the buttons and sliders went to their respective pins and I gave all of them a unique wire. After that I went back to coding and realized my original code didn't work because the I didn't use input pullup with ground and instead used input with 5v so at first random notes played without my control and when I tried playing a note, multiple notes would come out. I eventually figured it out and the potentiometers worked fine.   

<iframe width="800" height="450" src="https://www.youtube.com/embed/Sj6T5Gp7otA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

# First Milestone

My first milestone was managing to produce a MIDI sound by pressing a button and being able to adjust its volume through a potentiometer. Through coding, I managed to check when the button is being pressed and send out a Serial output which can be converted into MIDI. I also did the same for the potentiometer where it checks if there's a big enough change in the read of the potentiometer and then produce an output which can also be converted into MIDI. Through the MIDI message list, I learned what each of the number outputs does and that allowed the output to correspond with the correct function.

<iframe width="800" height="450" src="https://www.youtube.com/embed/5lB8M1C9zg4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

# Materials



https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/

https://www.amazon.com/SunFounder-Serial-Module-Display-Arduino/dp/B019K5X53O/

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Arduino Uno R3 |  | $25.94 | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> here </a> |
|:--:|:--:|:--:|:--:|
| LCD I2C | **Important** The SDA and SCL pins are connected to the A4 and A5 pins on the Uno R3, this means that if you are adding an LCD display, you cannot use the A4 and A5 pins at the same time | $11.99 | <a href="https://www.amazon.com/SunFounder-Serial-Module-Display-Arduino/dp/B019K5X53O/"> here </a> |
|:--:|:--:|:--:|:--:|
| Arcade Buttons | Without a mux, you can only use 12 buttons for the controller | $11.00 | <a href="https://www.amazon.com/Avisiri-Buttons-Replace-OBSF-24-Joystick/dp/B07X242Z4D/"> here </a> |
|:--:|:--:|:--:|:--:|
| Rotary Potentiometer | Without a mux, you can only use 4 of potentiometers **including** the sliders | $9.99 | <a href="https://www.amazon.com/dp/B07DHL77RT/"> here </a> |
|:--:|:--:|:--:|:--:|
| Slide Potentiometer |  | $13.99 | <a href="https://www.amazon.com/1100PCS-Headers-Connector-Housing-Ltvystore/dp/B07232HGS1/?th=1"> here </a> |
|:--:|:--:|:--:|:--:|
| Container | Any container will work, I just used a square cardboard box at first and then added a smaller one for the LCD, make sure to cut the holes smaller so that the buttons and potentiometer don't end up being wobbly | depends | depends 

# Tools

| **Tool** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Soldering Kit | $20.99 | <a href="https://www.amazon.com/Soldering-Iron-Kit-Temperature-Desoldering/dp/B07S61WT16/"> here </a> |
|:--:|:--:|:--:|:--:|
| Wire Strippers | $6.99 | <a href="https://www.amazon.com/gp/product/B097STWW4Q/ref=ox_sc_act_title_1?smid=AZ0MMPOLVYF3T&psc=1"> here </a> |
|:--:|:--:|:--:|:--:|
| 22 Gauge Wires | $14.94 | <a href="https://www.amazon.com/gp/product/B088KQFHV7/ref=ox_sc_act_title_2?smid=A2WIZBA4LZM5RA&psc=1"> here </a> |
