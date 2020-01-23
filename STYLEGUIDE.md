## Humanite (.hcode)

All code is written in Humanite, which means you don't have to think too much! Here's why:

## Is Humanite Java?

Well.. could be! Humanite is a syntax developed by Human Corp. and the compiler of it just understands what you wrote, however you did it. You could write some code in a PHP-like structure if you feel like it. The devs of the first leaks just like the Java-y structure.

```php
public function doAction($intent) { // This code is perfectly valid.
	BRAIN.CALL($intent->action)
}
```

So, just **write it however you want**! Just keep an eye on the original style of code when you refactor already writte code to make it less confusing.

## Event hooks

There's also a runtime call-event-hook system in place that can execute code before/on/after/parallel to/etc. another call. There's a lot of ways to let the compiler know of them, here is an example of one way that can be achieved:

```
@HookBefore(Person.putDown(Mug))
public void mightSpillEvent(Mug mug) {
	//...
}
```
