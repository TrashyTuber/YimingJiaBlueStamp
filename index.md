# MIDI Controller
Imagine that you want a piano just for fun but realize that they cost thousands of dollar and there's no way you will spend that much. This project here contains all the basic components of a digital piano and even an LCD display showing the volume and instruments selected. 

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Yiming Jia | Dougherty Valley High School | Electrical Engineering | Incoming Sophomore

![Headstone Image](https://bluestampengineering.com/wp-content/uploads/2016/05/improve.jpg)
  
# Final Milestone
My final milestone is the increased reliability and accuracy of my robot. I ameliorated the sagging and fixed the reliability of the finger. As discussed in my second milestone, the arm sags because of weight. I put in a block of wood at the base to hold up the upper arm; this has reverberating positive effects throughout the arm. I also realized that the forearm was getting disconnected from the elbow servo’s horn because of the weight stress on the joint. Now, I make sure to constantly tighten the screws at that joint. 



# Second Milestone
My second milestone was mainly making the box of the controller and soldering all the wires that connect the buttons to the arduino board. For the box, I didn't have the right tools to cut the circles for my buttons so I just used a compass to map it out and a small scissor to cut it. For the potentiometers and the sliders, the holes were to small to use a compass so I drew the point out and use a pencil to shove a hole out until it's big enough for the potentiometer to fit in. The soldering took a long time for me to get used to but I basically used one type of wire to connect up all the 5v and another for the ground. The other port of the buttons and sliders went to their respective pins and I gave all of them a unique wire. After that I went back to coding and realized my original code didn't work because the I didn't use input pullup with ground and instead used input with 5v so at first random notes played without my control and when I tried playing a note, multiple notes would come out. I eventually figured it out and the potentiometers worked fine.   

<iframe width="800" height="450" src="https://www.youtube.com/embed/Sj6T5Gp7otA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
# First Milestone
  

My first milestone was managing to produce a MIDI sound by pressing a button and being able to adjust its volume through a potentiometer. Through coding, I managed to check when the button is being pressed and send out a Serial output which can be converted into MIDI. I also did the same for the potentiometer where it checks if there's a big enough change in the read of the potentiometer and then produce an output which can also be converted into MIDI. Through the MIDI message list, I learned what each of the number outputs does and that allowed the output to correspond with the correct function.

<iframe width="800" height="450" src="https://www.youtube.com/embed/5lB8M1C9zg4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
