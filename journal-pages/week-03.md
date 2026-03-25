---
layout: default
---

# Week 03

[← Back to Home](../index.md)

## Documentation 

*Include your documentation for the week. Devise your own structure of headings relevant to the required tasks and your process.*

## Images & Media

*Use the format below to embed images from your assets folder:*

`![Alt text](../assets/week-01/your-image.jpg)`
`*Your caption here*`

*The text inside the square brackets is alt text (a description for accessibility), not a visible caption. To add a caption, place a line of italic text below the image.*

## AI Usage Statement

*Document any use of AI tools under an AI Usage Statement heading. Explain which tools you used and describe how you used them. Reference any AI-generated content (see [QuickCite](https://auckland.libguides.com/referencing-generative-ai-tools) for guidance).*

Friday 23 march - studio 2
overview of studio
We had to go through digital and analogue approaches and explore how to access, filter and translate live data into a visual and material forms. These activities build on from the coding fundamentals from experiment 2 
**Activity one**
For the first activity we had to explore with cURL using terminal and the documentation and try to figure out how to 
- Get the weather for a location using its GPS coordinates
- Get the weather in a different language
- Get the current moon phase
- Look up the synonyms and antonyms of a word
- Find something else in the documentation that we haven't covered
I started by locating where the terminal is on my computer and learning what each of the command does. For example cd shows me where i am, dir displays the directory contents of my computer and documents list all the documents i have 

From there i moved onto completing the list on using curl in the terminal. the first task was to get the weather for a location  using its gps coordinates. how it works is that when i run the command my terminal uses crul to send a request to wttr.in and wttr.in reads those coordinates to figure out where the location is. [weather](../assets/week-03/weather.png)

This is the same weather as the first one but this one is just in a different language. how this works i run a command which uses crul to send a request to wttr.in. The difference is that the ?lang=ko tells wttr.in which language i want the weather to be in and the server reads that language code (for example, es for Spanish, fr for French, ko for Korean) that is at the end of ?lang=ko and translates the weather descriptions into that language [weather korean](../assets/week-03/weather%20korean.png)

This is where it show the current moon phase we have and how this code works is just like the weather data but the only difference is the /moon at the end tells wttr.in that i don't want weather but the current moon lunar phase [moon phase](../assets/week-03/moon%20phase.png)  

this is the synonyms and antonyms of the word happy and how this code works is that my terminal uses curl to send a request to the free dictionary api which is asking for all the information it has on the word happy ans sends back a JSON response containing thing about the word happy  
[synonyms and antonyms](../assets/week-03/synonyms%20and%20antonyms.png)

something else in the doc that wasn't covered 

**Activity  two**
After that we got a demo sketch of the current weather data for auckland we were told to experiment with the sketch. So what i did was changed the latitude and longitude to a different city so from auckland new zealand i did tokyo japan. how the sketched change was instead of showing auckland weather i showed tokyos weather and how i new that was because the wind bar was much more lower then it had been for auckland.
[auckland](../assets/week-03/auckland.png)[tokyo](../assets/week-03/tokyo%20.png)

from there i went on and used the data to try an control different visual properties such as colour, position, size, and the number of shapes. so i went back to the auckland weather data and i first changed the colours of the circle and the temp bar 
[colour change](../assets/week-03/colour%20change.png) [colour change code](../assets/week-03/colour%20change%20code%20.png)

Then i changed the position of the circle to move it to the top right conner and wind bar more higher just under the circle making it look like a sunrise which fit in with this a it relate to weather.
[position](../assets/week-03/position%20.png)[position](../assets/week-03/position%20code%20.png)

From there i changed the size of the of the circle making the circle smaller and the rectangle bigger to make it look more like a sunset 
[size](../assets/week-03/size%20.png)[size code](../assets/week-03/size%20code%20.png) 

**Activity three**
For this activity we had to get into pairs and design a data protocol: a set of rules for translating a live dta source but since i wasn't there to do the in class activity i did it by myself as home and asked my flatmates to execute my protocol

The protocol must specify the source, frequency and mapping. The live data that i decided to observe was human movement in which i would observe the movement my flatmates make (e.g walk across a room, entering a room, leaving a room).  The frequency that i would count would every 15 seconds and this is how i would map it (photo of map)

I did this for 5 mintues and this was the result (photo of protocol result)

**Independent Study**
For this independent study we were to build on from the in class activities done to make a work that engages with live data. which meant we had to build a sketch in p5.js that would respond to live data.

