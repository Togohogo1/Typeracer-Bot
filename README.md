# TypeRacer-Bot
Python program that allows the use of both sending keys and simulating keypresses to cheat in TypeRacer. Be aware that the effectiveness of the program will depend on latency.  

![race](https://github.com/Togohogo1/TypeRacer-Bot/blob/master/screenshots/race.png)  
![interactive](https://github.com/Togohogo1/TypeRacer-Bot/blob/master/screenshots/interactive.png)  

### Setup
A webdriver is necessary for the program to run. If the ones located in `TypeRacer-Bot/drivers` do not work it probably means that either the browser version is not compatible with the webdriver version and/or the browser for the webdriver isn't installed. Driver downloads are available for [Chrome](https://chromedriver.chromium.org/downloads), [Firefox](https://github.com/mozilla/geckodriver/releases), [Edge](https://developer.microsoft.com/en-us/microsoft-edge/tools/webdriver/), and more.

To start the program, double click `run.bat` once downloaded. All necessary libraries will be installed in a virtual environment.

### Racing
Anytime a race starts, the user is asked to input a delay time. If nothing or something invalid is inputted, then the delay time is set to a default value. During the race, one of the two methods of typing, `send_text(driver, text, delay)` and `press_text(keyboard, text, delay)` will be used.

If using `send_text()`, the delay can be entered before the race starts because the program will automatically send the text to the inputbox when it is detected. This method is the one currently used in the program.

If using `send_text`, the delay must be entered as soon as the races start, and the inputbox must be manually selected before the program starts to simulate keypresses.

In `main(link, default, driver)`, `link` can be modified to open an invite link, `delay` can be modified to change the default delay time, and `driver` can be modified to either `chrome`, `firefox`, or `edge`. Additionally arguments can be passed in `main()` in the form of `param=value`.

### Todo
- Perhaps make the bot more automatic
- Efficiently implement more settings and display them
