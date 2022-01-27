
## PYTHON CODE FOR RASPBERRY PI DHT11/DHT22
Next thing we need to do is install the DHT python library. This is done by entering  the following command:
```
sudo pip3 install Adafruit_DHT1
```

Note: If you run into problems with the above command, you may not have PIP installed on your Pi.  You can fix that by running the following commands.  These will install PIP and other utilities you may need.

```
sudo apt-get install python3-dev python3-pip
sudo python3 -m pip install --upgrade pip setuptools wheel
```

OK. Now let’s take a look at the code we’re going to use. This is some very basic code written in Python. The first section of code imports the DHT library from Adafruit and the system time library.

```
import Adafruit_DHT
import time
```
This line defines the sensor object we will use, and the next line is a variable that defines the GPIO pin we are using.

```
DHT_SENSOR = Adafruit_DHT.DHT11
DHT_PIN = 4
```

And finally the code loop that goes next.  The “while True:” line will force everything indented after to run in an infinite loop.