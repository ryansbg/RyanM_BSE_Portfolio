# Ryan M's Blue Stamp Project - Air Quality Monitor with Active Buzzer and LED Alert System
Replace this text with a brief description (2-3 sentences) of your project. This description should draw the reader in and make them interested in what you've built. You can include what the biggest challenges, takeaways, and triumphs from completing the project were. As you complete your portfolio, remember your audience is less familiar than you are with all that your project entails!

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Ryan M | Los Gatos High School | Electrical, Mechanical, Software Engineering | Incoming Sophomore

**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**

![Headstone Image](logo.svg)
  
# Final Milestone
For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

# Second Milestone
For your second milestone, explain what you've worked on since your previous milestone. You can highlight:
- Technical details of what you've accomplished and how they contribute to the final goal
- What has been surprising about the project so far
- Previous challenges you faced that you overcame
- What needs to be completed before your final milestone 

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/y3VAmNlER5Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

# First Milestone
For my first milestone, I experimented with and learned about all the parts included in the Super Starter Kit. Since this was my first experience with coding and using a breadboard, I spent a significant amount of time learning about the code and how to use the breadboard. The goal of my first milestone was to complete the base product, and I did that. I completed my build of an MQ135 air quality monitor with an OLED display, and troubleshot coding issues regarding resistor variable values in the MQ135 to finalize the code. A challenge I'm sure I will face in future milestones is that I will have to be careful when combining the code for different parts like the LED and Active Buzzer with the code for the base AQ monitor. I'm sure this will pose a challenge for me. My plan for the second milestone is to have somewhat of a working prototype for my final product, with an LED and Active Buzzer connected to the base product and somewhat working.

<iframe width="560" height="315" src="https://www.youtube.com/embed/j5LZdaHLu88" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

# Schematics 
Milestone 3 Final Schematic (Base Product + LED/Buzzer/Temp and Humidity Module)

![Headstone Image](MS3_Schematic.png)

Milestone 2 Schematic (Base Product + LED/Buzzer)

![Headstone Image](MS2_Schematic.png)

Milestone 1 Schematic (Base Product)

![Headstone Image](MS1_Schematic.png)

Schematics Notes:
Tinkercad did not have a lot of the parts I used, so I did my best to replace them with the parts it had. The Temperature Sensor in the schematic is actually the DHT11 Temperature and Humidity Module, which is why the pins are rearranged (power and data pin are switched), the Gas Sensor is the MQ135 Air Quality Module (ignore the bottom three pins on the gas sensor), and the large OLED display is actually a smaller OLED display with only four pins that connect to analog pins on the Arduino, which is why there is only four connected in the schematic. Also, the piezo is the active buzzer, and the setup of the actual product is a little bit different than the schematic.
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
| Arduino UNO Rev3 | Write and run code to deliver to connected devices | $28.50 | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
|:--:|:--:|:--:|:--:|
| Solderless Breadboard | Used to create temporary circuits and to connect electrical components together | $9.99 (3pcs) | <a href="https://www.amazon.com/EL-CP-003-Breadboard-Solderless-Distribution-Connecting/dp/B01EV6LJ7G/ref=asc_df_B01EV6LJ7G?tag=bingshoppinga-20&linkCode=df0&hvadid=80539278509443&hvnetw=o&hvqmt=e&hvbmt=be&hvdev=c&hvlocint=&hvlocphy=&hvtargid=pla-4584138857801087&psc=1"> Link </a> |
|:--:|:--:|:--:|:--:|
| OLED SSD1306 128x64 LCD Display | Used to display ppm values detected by air quality monitor | $8 | <a href="https://www.walmart.com/ip/0-96-OLED-SSD1306-I2C-IIC-SPI-Serial-128X64-LCD-Display-Gelb-Blau-LCD-5Q8K-C9H1/1079180220?wmlspartner=wlpa&selectedSellerId=101255994&adid=22222222222000000000&wmlspartner=wmtlabs&wl0=e&wl1=o&wl2=c&wl3=10352200394&wl4=pla-1103028060075:aud-813964392&wl5=&wl6=&wl7=&wl10=Walmart&wl11=Online&wl12=1079180220_10001275354&wl14=SSD1306%20128x64%20OLED%20LCD&veh=sem&gclid=9207663575fc180c1add02a50be3edbd&gclsrc=3p.ds&msclkid=9207663575fc180c1add02a50be3edbd"> Link </a>|
|:--:|:--:|:--:|:--:|
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
|:--:|:--:|:--:|:--:|

# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [MQ135 Code and Setup Help](https://steemit.com/utopian-io/@cha0s0000/arduino-basics-tutorials-use-mq135-air-quality-detecting-module)
- [Coding Help for Milestone 1](https://arduino.stackexchange.com/questions/26832/how-do-i-convert-a-float-into-char)
- [Understanding OLED Display](https://www.youtube.com/watch?v=rxjIXVwgY50)

To watch the BSE tutorial on how to create a portfolio, click here.
