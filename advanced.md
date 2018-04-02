# Different JVM Languages

Methods allow you to smoothly display code examples in different JVM languages.

{% method %}
## My first method

My first method exposes how to print a message in Java and Kotlin.

{% sample lang="java" %}
Here is how to print a message to `stdout` with Java.

```java
System.out.println("My first method");
```

{% sample lang="kotlin" %}
Here is how to print a message to `stdout` with Kotlin.

```kotlin
fmt.Println("My first method")
```

{% common %}
Whatever language you are using, the result will be the same.

```bash
$ My first method
```
{% endmethod %}
