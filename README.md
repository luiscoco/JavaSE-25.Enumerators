# JavaSE-Enumerators

See the Udemy course: https://www.udemy.com/course/curso-certificacion-profesional-desarrollador-java-se-11

In Java, an enumerator, or more commonly known as an enumeration or enum, is a special data type that consists of a set of named constants. 

Enumerations make code more readable and maintainable by providing a way to represent a fixed set of values.

Here's a simple example to illustrate enumerators in Java:

```java
// Define an enumeration named Color
enum Color {
    RED, GREEN, BLUE;
}

public class EnumExample {
    public static void main(String[] args) {
        // Using enum constants
        Color myColor = Color.RED;

        // Switch statement with enum
        switch (myColor) {
            case RED:
                System.out.println("I love red!");
                break;
            case GREEN:
                System.out.println("Green is refreshing.");
                break;
            case BLUE:
                System.out.println("Feeling blue today.");
                break;
        }

        // Iterate through all enum constants
        System.out.println("All colors:");
        for (Color color : Color.values()) {
            System.out.println(color);
        }
    }
}
```

In this example, we have defined an enumeration Color with three constants: RED, GREEN, and BLUE. You can use these constants in your code to represent specific colors.

The main method demonstrates how to use the enum. We create a variable myColor of type Color and assign it the value Color.RED. We then use a switch statement to perform different actions based on the color.

The for loop at the end shows how to iterate through all the constants of the enum using the values() method.

Enums are useful when you have a fixed set of related constants, and they provide better type safety compared to using plain integers or strings for such cases.
