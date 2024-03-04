**Advanced working with functions**

- [Scheduling](#scheduling)
  - [setTimeout](#setTimeout)
  - [setInterval](#setInterval)
- [Decorators](#decorators)
  - [Spy](#spy)
  - [Debounce](#debounce)
  - [Throttle](#throttle)




# Scheduling



# Decorators
- JS gives flexibility when dealing with functions. **They can be passed around, used as objects, and forward calls between them and decorate them**
- **Decorators can be seen as “features” or “aspects” that can be added to a function. We can add one or add many. And all this without changing its code**
- Decorator is a wrapper around a function that alters its behavior. The main job is still carried out by the function.
- Throttling and debouncing are two ways to optimize event handling
- Throttling and debouncing **are two most common ways to control a listener response rate to an event**

## Throttle
Throttling is the **action of reducing the number of times a function can be called over time to exactly one.**

For example, if we throttle a function by 500ms, it means that it cannot be called more than once per 500ms time frame. Any additional function calls within the specified time interval are simply ignored.

When to use throttle?

Use throttling to consistently react to a frequent event.

This technique ensures **consistent function execution within a given time interval.** Since throttle is bound to a fixed time frame, the event listener should be ready to accept an intermediate state of the event.

Common use cases for throttling include:
- Any consistent UI update after window resize
- Performance-heavy operations on the server or client

## Debounce
**A debounced function is called after N amount of time passes since its last call.** It reacts to a seemingly resolved state and implies a delay between the event and the handler function call.

When to use debounce? Use debounce to eventually react to a frequent event.

Debounce is useful when you don't need an intermediate state and wish to respond to the end state of the event. That being said, you need to take into account an inevitable delay between the event and the response to it when using debounce.

Common use cases for a debounced function:
- **Asynchronous search suggestions**
- **Updates batching on the server**









