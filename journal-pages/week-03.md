[← Back to Home](../index.md)

Friday 20 march - studio 3
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

From there i moved onto completing the list on using curl in the terminal. the first task was to get the weather for a location  using its gps coordinates. how it works is that when i run the command my terminal uses curl to send a request to wttr.in and wttr.in reads those coordinates to figure out where the location is. 
[weather](../assets/week-03/weather.png)

This is the same weather as the first one but this one is just in a different language. how this works i run a command which uses curl to send a request to wttr.in. The difference is that the ?lang=ko tells wttr.in which language i want the weather to be in and the server reads that language code (for example, es for Spanish, fr for French, ko for Korean) that is at the end of ?lang=ko and translates the weather descriptions into that language [weather korean](../assets/week-03/weather%20korean.png)

This is where it show the current moon phase we have and how this code works is just like the weather data but the only difference is the /moon at the end tells wttr.in that i don't want weather but the current moon lunar phase [moon phase](../assets/week-03/moon%20phase.png)  

this is the synonyms and antonyms of the word happy and how this code works is that my terminal uses curl to send a request to the free dictionary api which is asking for all the information it has on the word happy and sends back a JSON response containing thing about the word happy  
[synonyms and antonyms](../assets/week-03/synonyms%20and%20antonyms.png)

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

For this activity we had to get into pairs and design a data protocol: a set of rules for translating a live data source but since i wasn't there to do the in class activity i did it by myself as home and asked my flatmates to execute my protocol

The protocol needed to specify the source, the frequency and the mapping. for the live data source i had chose to observe the human movements that were happening in my flat such as moving across the room, entering or leaving the room. i made the observation every 15 seconds  and made a map to translate the movement. we were suppose to swap protocols with other and since i was working alone i wasn't able to so i just foolowed my own. [protocol map](../assets/week-03/protocol%20map.jpg)

I completed this protocol for 3 minutes because i wasn't sure on how long i was meant to run this for. i also used a timer to keep it consistent and this was the outcome. 
[protocol data](../assets/week-03/protocol%20data.jpg)

we were to answer these question about the other people's protocol
Did you interpret the rules as they expected? Where was the protocol ambiguous? What surprised you about the result?
but since i was the only one doing it i answered the questions as if someone else had written it.

for the most i did interpret the rules as they expected it had a basic structure, checking every 15 seconds and recording movement using the symbols was straightforward that i could follow it consistently  

there were areas that felt unclear once i tired to follow the instructions like the symbol for 2 people moving could have be misread as a number rather then being a mapping symbol. simultaneous movement were tricky like if someone entered the room while someone else walked across the room as the protocol didn't specify which symbol should take priority and which one should be wrote down first.

what surprised me was how quickly the a page filled up with symbols and how abstract the final outcome of the protocol looked. 

**Independent Study**

For this independent study we were to build on from the in class activities done to make a work that engages with live data. which meant we had to build a sketch in p5.js that would respond to live data.

i found a API to work with and to build a sketch that would responds to live data which is a dog API where every second people are adding there dogs the a open source dog pictures. 

For the coding of the api i used the weather code from activity two to help me structed the code for the dog Api. And before starting to code i did look at some for the references like loading JSON, loading images, preload,typography to give me an idea of how to code the dog API. Once i got the basic sense of what i needed to do i started to code.

so the first part of the code was the variables and API url where is sets up the three variables, one to store the dog image, one for the api endpoint and the last one for the background colour. together they will establish the data flow for the sketch.
[variables](../assets/week-03/variables.png)

This next part of the code was the preload where it makes sure the first image of the dog is fully loaded before that sketch begins.
[preload](../assets/week-03/preload.png)

This part of the code was the setup where it creates the canvas and configures how the images and test should align. and the button where it adds a button that lets the user get a new dog image whenever that click it and makes the canvas
[setup](../assets/week-03/setup.png)

This part of the code was load new dog where extracts the image url from JSON, loads the images and maps the url to a background color.
[load new dog](../assets/week-03/load%20new%20dog.png)

This is the last part of the code where it draws, displaying the dog image and background and this where is sets the background colour, displays the dog images if it is loaded and shows the loading messages if the dog image hasn't loaded yet.
[draw](../assets/week-03/draw.png) 

overall i found i pretty easy to code as i did the weather code and references from p5.js which helped alot when i start to code the dog api

**Reflective writing**

For the independent study i took the digital approach as i felt it would be alot more easier to do then the analogue/physical approach as i felt i would have taken alot more time creating and trying to make it perfect without leaving me enough time to document the process where with the digital approach i felt i could get it done in a appropriate amount of time and still have enough time to do the document the process

The live data source that i worked with was a dog api which was the internet's biggest collection of open source dog pictures where people would continuously add photos of there dogs. how i accessed was i first figured out what api i wanted to use and i wanted something related to animals from there i chose to do it related to dogs as i am a dog lover. So then i searched up dog apis that the one that i used was the first one to pop up so i went with that.

Because the dog api really only had one piece of data being a random dog image i focused on making the data visually interesting to look at. With the dog image being mapped out onto the canvas and the background being a colour. 

What my work reveals is that even the most simple data like the dog api can make a meaningful variation 

the way that i coded was in a structured form as i feel that vide coding is just not for me as for when i code i need to have structure as where i learned with vide coding you go with the flow and i feel like it is to confusing and overwhelming or me to do. 

My work relates to the practitioner because it uses live data an simple rule like David Bowen where is relies on the unpredictable data like a random dog images or like conditional design by using simple rules, get a dog image, map the url length to colour.

What i would like to develop further with more time is the background colour changing each time the image of the dog changes as i feel it would be visually interesting to look at.