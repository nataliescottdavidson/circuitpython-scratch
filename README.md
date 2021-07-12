 # circuitpython-scratch

 Playing with the adafruit NeoTrellis lil synth / macropad type thing

 Have it hooked up to my macbook pro currently, working through finding the correct IC2 address. 

 These [libraries](https://github.com/adafruit/Adafruit_CircuitPython_Bundle) are needed

 Hmm so I2C scan is coming up empty when NeoTrellis connected to my macbook. https://learn.adafruit.com/circuitpython-basics-i2c-and-spi/i2c-devices

 But `list_ic2_scl_pins.py` shows up with a bunch of pins. Output is 

 ```
 SCL pin: board.A1 	 SDA pin: board.A2
SCL pin: board.ACCELEROMETER_SCL 	 SDA pin: board.ACCELEROMETER_SDA
SCL pin: board.ACCELEROMETER_SDA 	 SDA pin: board.ACCELEROMETER_SCL
SCL pin: board.ACCELEROMETER_SDA 	 SDA pin: board.SDA
SCL pin: board.COL2 	 SDA pin: board.COL3
SCL pin: board.COL2 	 SDA pin: board.COL6
SCL pin: board.COL3 	 SDA pin: board.COL2
SCL pin: board.COL6 	 SDA pin: board.COL7
SCL pin: board.COL6 	 SDA pin: board.APA102_SCK
SCL pin: board.COL7 	 SDA pin: board.COL3
SCL pin: board.COL7 	 SDA pin: board.COL6
SCL pin: board.APA102_MOSI 	 SDA pin: board.COL7
SCL pin: board.APA102_MOSI 	 SDA pin: board.APA102_SCK
SCL pin: board.SCL 	 SDA pin: board.ACCELEROMETER_SCL
SCL pin: board.SCL 	 SDA pin: board.SDA
 ```

 Ack. I don't get why it doesn't work when it is clearly connected somehow. Going to try with my Pi as the client next.
