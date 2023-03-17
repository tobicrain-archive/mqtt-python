Python MQTT/InfluxDB Publisher and Subscriber Application
=========================================================

This is a Python desktop application that allows you to publish and subscribe to MQTT topics, and save retrieved messages to an InfluxDB database. The application has a command-line interface and provides a simple way to interact with the MQTT broker and InfluxDB database.

Prerequisites
-------------

To run this application, you need to have the following software installed on your computer:

*   Python 3.7 or higher
*   Eclipse Paho MQTT client library for Python
*   InfluxDB Python client library

You also need to have access to an MQTT broker and an InfluxDB database.

Getting Started
---------------

1.  Clone the repository to your local machine.
    
2.  Install the required Python libraries:
    
    bashCopy code
    
    `pip install paho-mqtt influxdb`
    
3.  Set up the MQTT broker and InfluxDB database connection in the `config.ini` file.
    
4.  Run the application.
    

Using the Application
---------------------

### Publisher

To publish a message, follow these steps:

1.  Enter the MQTT topic and message as command-line arguments.
    
    bashCopy code
    
    `python publisher.py <topic> <message>`
    

The message will be sent to the MQTT broker.

### Subscriber

To subscribe to a topic and retrieve messages, follow these steps:

1.  Enter the MQTT topic as a command-line argument.
    
    bashCopy code
    
    `python subscriber.py <topic>`
    

The application will start listening to the MQTT broker for messages published to the specified topic. The retrieved messages will be saved to the InfluxDB database.

License
-------

This application is licensed under the MIT License. See the LICENSE file for details.
