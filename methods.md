# Defining Methods

Methods allow you to smoothly display code examples in different JVM languages.

{% method %}
## My first method

My first method exposes how to print a message in Java and Go.

{% sample lang="java" %}
Here is how to print a message to `stdout` using Java.

```js
console.log('My first method');
```

{% sample lang="go" %}
Here is how to print a message to `stdout` using Go.

```go
fmt.Println("My first method")
```

{% common %}
Whatever language you are using, the result will be the same.

```bash
$ My first method
```
{% endmethod %}
