# ts-uploader
Upload your Sensor Data to Thingspeak using this program and your Arduino board by USB. 
Written under Processing 2.2.1

In order to use this program:

1)you need to create a ThingSpeak account (www.thingspeak.com)

2)Create a channel with at least 3 charts on it. 

3)Then you need to generate an API key for writing values to the charts. 

4) COPY THE API KEY INSIDE THE "api.txt" FILE IN THE DATA DIRECTORY.

5) Load the sketch to the Arduino Board. 

5.1) Yo can creae your own version of the Arduino sketch according to your needs. The program requires a Serial input as follows:
 Serialprintln("value1,value2,value3,value4,value5,value6,value7,value8");
 delay(t); //where t should be at least 15 seconds.
 
 Each value goes to a different field in the Thingspeak channel.
 IF YOU SEND LESS VALUES, LEAVE THE SPACE BETWEEN COMMAS EMPTY. Example: (value1,value2,,,,,,)
 
