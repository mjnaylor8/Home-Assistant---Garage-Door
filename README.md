# Home-Assistant---Garage-Door
Helper and Automations for Garage Door


This was inspired by https://www.speaktothegeek.co.uk/2023/06/esphome-smart-garage-door-controller/.

However I found the Home Assistant Cover did not do what I wanted and so decided to develop my own 'opener'.  The code will not be the best fully optimised code there is but it works for me!

Based on a D1 Mini ESP8266 Dev Board microcontroller a Relay Module 1Ch 5V with Optocoupler and a reed switch all purchased from https://www.bitsboxuk.com/.
I used ESP Home to programme the D1 Mini.

The actions mimic using a button on the wall in the garage / or the garage door remote.

The door using the button works as follows:-
1.  Door Closed....
  - button press - door opens

2.  Door Open....
  - button press - door closes

3.  Button pressed when opening or closing
  - button press - door stops
    if door opening
    button press - door closes
    if door closong
    button press - door opens

The D1 Mini triggers the relay which mimics the door button press action.

<img width="388" alt="Screenshot 2025-03-13 at 16 15 42" src="https://github.com/user-attachments/assets/70055880-aa54-4ded-b49c-df66222b7dd6" />

The image above shows the custom button
Title
Icon - changes as door opens and stops
Status - changes and door open and stops
Slider and numeric % - showing position of door
Icon - showing the action of the next button press


