# Getting Started with Indriya

In this chapter, we'll explain how to set up a simple Maven project and create your first quantity. Once you've done that, you're all set to explore the rest of the functionality of Indriya.

## Setting Up Your Maven Project

In order to be able to use Indriya, you first have to set up your Maven project correctly. Assuming you have a working POM file, all you should need to do is to add the following dependency to your project:

```markup
    <dependency>
      <groupId>tech.units</groupId>
      <artifactId>indriya</artifactId>
      <version>2.0.4</version>
    </dependency>
```

## Your First Quantity

Next, we'll create a Java class that will create your first quantity, the speed of light \(_c_\). Let's start by creating a new class in a package of your choice. In that class, import the following types in order to create a new speed quantity:

```java
import javax.measure.Quantity;
import javax.measure.quantity.Speed;

import tech.units.indriya.quantity.Quantities;
import tech.units.indriya.unit.Units;
```

In order to keep things simple, we'll create the quantity in the class's `main` method, and print it out immediately.

```java
  public static void main(String[] args) {
    Quantity<Speed> C = Quantities.getQuantity(1079252849, Units.KILOMETRE_PER_HOUR);
    System.out.println("The speed of light: " + C);
  }
```

Compile the class, and run it as a stand-alone Java application. The result should be like this:

```text
The speed of light: 1079252849 km/h
```

That's it: you've just included Indriya as a dependency to a project, and created and printed out your first quantity!

