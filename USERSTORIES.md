User Stories and process
============

```
As an air traffic controller
So I can get passengers to a destination
I want to instruct a plane to land at an airport and confirm that it has landed
```
Object | Message
------- | -------
air_traffic_controller |
passenger |
plane | landed?
airport | land

**Notes:**

Originally created the method to return the string "Plane has landed", but I didn't think that it fully completed met the criteria so added the .landed? method to the plane class.

```
As an air traffic controller
So I can get passengers on the way to their destination
I want to instruct a plane to take off from an airport and confirm that it is no longer in the airport
```
Object | Message
------ | -------
air_traffic_controller |
passenger |
plane | taken_off
airport | take_off?

**Notes:**

Changed all the class methods that I had created. Now Airplane has the method .land which takes airport as an argument. Originally Airport was passed the .land method with an instance of plain as an argument. Had to rewrite all the tests. Created a test that checks if .take_off and .land alter the planes array in the Airport instance.

```
As an air traffic controller
To ensure safety
I want to prevent takeoff when weather is stormy

As an air traffic controller
To ensure safety
I want to prevent landing when weather is stormy

As an air traffic controller
To ensure safety
I want to prevent landing when the airport is full

As the system designer
So that the software can be used for many different airports
I would like a default airport capacity that can be overridden as appropriate
```