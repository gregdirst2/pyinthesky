# Welcome to lesson #3

## Getting started with Python on Arduino

### Objectives:
- Get aquanted with Python
- Intgrate Python with the Arduino
- Write your first Python code
- Make the onboard LED turn on and off

I found it easier to follow the guide and refer to the video when needed. The video only has music and plays very fast. You can slow this down if you like in YouTube under settings --> Playback speed.

[![Playback speed](https://github.com/StateFarm-STEM/pyinthesky/blob/main/lesson3-new/screenshots/yotube-settings-playback-speed.png)

### Guide
[Using Arduino with Python – Controlling Arduino’s LED with Python](https://www.electronicshub.org/controlling-arduino-led-python/)

There are a few gotchas once you get to the part where you are trying to Run the module since the Python and pySerial versions have changed since this video was published. I call them out below with the fixes.

### Issues and fixes

Invalid syntax - ensure all the print statements use parenthesis<br>
```print (Arduino_Serial.readline())```

raw_input not defined - change raw_input to just input<br>
```input_data = input()```

Unicode issue after pressing a number<br>
```Arduino_Serial.write(input_data.encode())```

### Video
[![the video](https://img.youtube.com/vi/4wWqka4EbEY/0.jpg)](https://www.youtube.com/watch?v=4wWqka4EbEY "click to watch")

### Python source code

[Lesson 3 Source Code](https://github.com/StateFarm-STEM/pyinthesky/blob/main/lesson3-new/python-workspace/lesson3-source/arduino-python-controll-the-led.py)
