# Online-Car-Rental-System

Username: admin
Password: 123

A car rental is a vehicle that may be rented for a price and utilized for a specific amount of time. Getting a rental automobile makes it easier for people to travel around when they don't have access to their own vehicle or don't own one at all. A person who needs transportation must call a rental car company and sign a contract. This method improves client retention while also making car and employee management more straightforward. 

We have created a web-based system that allows consumers to register and reserve automobiles online while also allowing the firm to manage its car rental business efficiently in order to make the process of renting an automobile easier for consumers.

-> Tools and Frameworks Used:

Swing

Java Swing is part of Java Foundation Classes. It is used to create window-based applications which makes it suitable for developing lightweight desktop applications. Java Swing is built on top of an abstract windowing toolkit API purely written in Java programming language.

Netbeans

NetBeans IDE is a free and open source integrated development environment for application development on Windows, Mac, Linux, and Solaris operating systems. The IDE simplifies the development of web, enterprise, desktop, and mobile applications that use the Java and HTML5 platforms.

Java Abstract Window Toolkit

Abstract Window Toolkit (AWT) is a set of application program interfaces ( API s) used by Java programmers to create graphical user interface ( GUI ) objects, such as buttons, scroll bars, and windows. AWT features include: A set of native user interface components. A robust event-handling model. Graphics and imaging tools, including shape, color, and font classes.

Database:

We are storing the data in .ser files

.ser files are mainly used to store serialized objects of a Java program. They also store metadata such as timestamps. They are used to store the objects after the program is terminated.

Java object Serialization is an API provided by Java Library stack as a means to serialize Java objects. Serialization is a process to convert objects into a writable byte stream. Once converted into a byte-stream, these objects can be written to a file. The reverse process of this is called de-serialization.

A Java object is serializable if its class or any of its superclasses implement either the java.io.Serializable interface.

The objects can be converted into byte-stream using java.io.ObjectOutputStream. In order to enable writing of objects into a file using ObjectOutputStream, it is mandatory that the concerned class implements Serializable interface as shown in the class definition below.

Reading objects in Java are similar to writing object using ObjectOutputStream and ObjectInputStream.



-> Design Principles and Design Patterns Applied
 
Single Responsibility Principle:

Each class should be responsible for a single part or functionality of the system. We have defined seperate classes for each functionality.

Open-Closed Principle:

In CarOwner.Java file, public class CarOwner extends Person implements Serializable. Hence it is open for extension.

Decorator Design Pattern:

Decorator design pattern is used to modify the functionality of an object at runtime. At the same time other instances of the same class will not be affected by this, so individual object gets the modified behavior. 
Suppose we want to implement different conditions of cars – we can create interface Car to define the assemble method and then we can have a Basic car, further more we can extend it having different conditions like Excellent, Good, Average and Bad.
