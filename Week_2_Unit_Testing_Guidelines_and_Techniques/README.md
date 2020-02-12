# UCSD Extension: Unit Testing: Supporting Modern Software Development Methods

## Videos: 

[Lecture 2: Unit Testing Guidelines and Techniques](URL link here)

## Assignment/Classwork:

Quiz #2 (Canvas)

Exercise 1:  

JUnit Run (Not Graded)

This exercise will help you get up and running with JUnit.
1. Create a new empty project using the build tool of your choice (Maven, Gradle). Add required
JUnit dependencies. Create a simple test class with a single test method containing some assertions.
2. Compile and run the test using your build tool.
3. Compile and run the test using your IDE.
4. Browse the test results.

Exercise 2:

Learn About AssertJ (Not Graded)
 
The simplest way to learn about assertions provided by AssertJ is the following. Open your IDE and
create a new test class. Then create a test method like this:

## Example:

```java
@Test
void learnAssertJ() {
 double var = 2.5;
 assertThat(var).
}
```
If you set the cursor after the hanging dot and ask your IDE for autocompletion then it will provide
you with the list of available methods. All you have to do now is to change the type of variable var to
String, BigDecimal or List<Object> and see what assertions are available.

Exercise 3:

Fahrenheits to Celcius with Parameterized Tests

A simple test class is shown below. Your task is to introduce parameterized tests, so there
will be no repetition in the test code.

```java
public class FahrenheitCelciusConverterTest {
    
@Test
 void shouldConvertCelciusToFahrenheit() {
    assertThat(FahrToCelcConverter.toFahrenheit(0)).isEqualTo(32);
    assertThat(FahrToCelcConverter.toFahrenheit(37)).isEqualTo(98);
    assertThat(FahrToCelcConverter.toFahrenheit(100)).isEqualTo(212);
 }
 
@Test
 void shouldConvertFahrenheitToCelcius() {
    assertThat(FahrToCelcConverter.toCelcius(32)).isEqualTo(0);
    assertThat(FahrToCelcConverter.toCelcius(100)).isEqualTo(37);
    assertThat(FahrToCelcConverter.toCelcius(212)).isEqualTo(100);
  }
 }
``` 
Exercise 4: 

Master Your IDE (Not Graded)

Make sure you spend some time learning about the support your IDE can give you in terms of
effective unit testing.

## Topics Covered: 

o	What is a Unit Test?

o	Interactions in unit tests

o	Writing unit tests


## Supplementary Items (Please Read!)

[JUnit 5 User Guide](https://junit.org/junit5/docs/current/user-guide/)

[AssertJ](https://assertj.github.io/doc/)

[Unit Testing Example (Similar to one used in presentation)](http://junit.sourceforge.net/doc/testinfected/testing.htm)

[DRY Principle](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself)

[Dependency Injection](https://en.wikipedia.org/wiki/Dependency_injection)
