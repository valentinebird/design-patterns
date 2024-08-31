#Adapter

Adapter is a structural design pattern, which allows incompatible objects to collaborate.

The Adapter acts as a wrapper between two objects. It catches calls for one object and transforms them to format and interface recognizable by the second object.

Usage examples: The Adapter pattern is pretty common in Java code. It’s very often used in systems based on some legacy code. In such cases, Adapters make legacy code work with modern classes.

There are some standard Adapters in Java core libraries:

java.util.Arrays#asList()
java.util.Collections#list()
java.util.Collections#enumeration()
java.io.InputStreamReader(InputStream) (returns a Reader object)
java.io.OutputStreamWriter(OutputStream) (returns a Writer object)
javax.xml.bind.annotation.adapters.XmlAdapter#marshal() and #unmarshal()
Identification: Adapter is recognizable by a constructor which takes an instance of a different abstract/interface type. When the adapter receives a call to any of its methods, it translates parameters to the appropriate format and then directs the call to one or several methods of the wrapped object.

Fitting square pegs into round holes

This simple example shows how an Adapter can make incompatible objects work together.