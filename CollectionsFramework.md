# The collections
===
- A collection = container = an object that groups multiple elements is single unit.

# The collections framework in java
===
- A Collections framework is used to store retrieve and manipulate aggregate data.
A Collections framework contains the following :
- Interfaces :
- Implementations :
- Algorithms :



# Interface, class, extends, implements . . . </br>Who does what?
===
- An interface cannot implement another interface.</br>
  ```java
  public interface A {
    // method signatures
  }
  public interface B  ~~implements~~ A ---> invalid {}
  ```
  Unlike word "implements" suggests, we are not implementing any method in interface B, hence, not allowed.
- One interface and extend one or more interfaces.

  ```java
  public interface C {
    // method signatures
  }

  public interface B extends A, C {
    // method signatures
  }
  ```
- One class can implement one or more interfaces.
  ```java
  public class D implements A, C {
    // method implementations
  }

  public abstract class E implements A, C {
    // 0 or more method implementations
  }
  ```
- A class cannot extend multiple classes. A class can extend only one parent class.
  ```java
  public class F {
    // method implementations
  }
  public class G {
    // method implementations
  }
  public class H ~~extends~~ F, G {} --> Invalid

  public class H extends G {} --> Valid
  ```
