# DesignPatterns
https://youtube.com/watch?v=tAuRQs_d9F8

## Creational Pattern 
1. Factory
2. Builder
3. Singleton

## Behavior Pattern
1. Observer / PubSub
It's common for different components of an app to respond to events or state changes, but how can we communicate these events?
The Observer pattern is a popular solution. We have a Subject (aka Publisher) which will be the source of events. And we could have multiple Observers (aka Subscribers) which will recieve events from the Subject in realtime.

In this case we have multiple Subscribers listening to a single published. But users could also be subscribed to multiple channels.
Since the Publishers & Subscribers don't have to worry about each others' implementations, they are loosely coupled.

2. Iterator
Many objects in python have built-in iterators. That's why we can conveniently iterate through an array using the key word in.

3. Strategty
A Class may have different behaviour, or invoke a different method based on something we define (i.e. a Strategy). For example, we can filter an array by removing positive values; or we could filter it by removing all odd values. These are two filtering strategies we could implement, but we could add many more.

## Structural Patterns


1. Adapter
Adapters allow incompatible objects to be used together. Following the Open-Closed principle, we can extend class behaviour without modifying the class itself.
If a MicroUsbCable class is initially incompatible with UsbPort, we can create a wrapper class (i.e. an Adapter), which makes them compatible. In this case, a MicroToUsbAdapter makes them compatible, similar to how we use adapters in the real-world.


2. Facade
According to Oxford Languages, a Facade is
`an outward appearance that is maintained to conceal a less pleasant or creditable reality.`
In the programming world, the "outward appearance" is the class or interface we interact with as programmers. And the "less pleasant reality" is the complexity that is hidden from us.
So a Facade, is simply a wrapper class that can be used to abstract lower-level details that we don't want to worry about.