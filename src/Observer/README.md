#Observer
Observer is a behavioral design pattern that allows some objects to notify other objects about changes in their state.

The Observer pattern provides a way to subscribe and unsubscribe to and from these events for any object that implements a subscriber interface.

Usage examples: The Observer pattern is pretty common in Java code, especially in the GUI components. It provides a way to react to events happening in other objects without coupling to their classes.

Here are some examples of the pattern in core Java libraries:

java.util.Observer/java.util.Observable (rarely used in real world)
All implementations of java.util.EventListener (practically all over Swing components)
javax.servlet.http.HttpSessionBindingListener
javax.servlet.http.HttpSessionAttributeListener
javax.faces.event.PhaseListener
Identification: The pattern can be recognized if you see a subscription method that stores incoming objects in a list. You can confirm the identification, if you see some sort of notification method that iterates over objects in that list and calls their “update” method.