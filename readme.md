# Day 1

## Java review contents

- [1-day Java review hands-on lab document](https://github.com/sashinpivotal/dsa-java-review-doc)
- [1-day Java review hands-on lab solution code](https://github.com/sashinpivotal/dsa-java-review-code)

## Java questions (Sang asks these questions to gauge students' Java knowledge)

- When do you want to use Java interface?
- When is a static method?  Why do you want to create a method as a static method? Is it a good idea to create a static method which maintains a state?
- What is encapsulation? What is abstraction?
- What is Polymorphism? What are the examples of polymorphism?
- What are the major differences between Set vs List?
- What is difference between "protected" vs "package private or default" access modifier?
- What is "Single responsibility principle of SOLID"? Why should we use it?
- What is "Open for extension Closed for modification of SOLID" design principle?
- What is dependency injection and why it is such an important software design concept?
- What is a functional interface in Java?
- What is Lambda expression? Where do you want use it?
- What is Generics and why you want to use it in your code?
- What is the difference between Java Collection vs Java Streams? (We are NOT talking about Java I/O Stream.)
- What is Optional class for in Java?
- What is a design pattern? What is "Strategy" pattern?
- What is dependency management in your project?

## Java resources (in addition to class provided ones)

- [Sang Shin's Java presentations](https://github.com/sashinpivotal/java-presentations)

## Individual (or group) tutorial sign-up sheet

- Two 30-minute slots are available before the class
- Please make sure to sign up the day before the tutorial session
- [Sign-up sheet](https://docs.google.com/document/d/1ZC7L3Zd1LXeG40vW3fA0k4TRCLETNHrWI13BPLt2z74/edit)

## .gitignore example file

```
# Operating System Files

*.DS_Store
Thumbs.db
*.sw?
.#*
*#
*~
*.sublime-*

# Build Artifacts

.gradle/
build/
target/
bin/
out/
dependency-reduced-pom.xml

# Eclipse Project Files

.classpath
.project
.metadata
.loadpath
bin/
.settings/

# IntelliJ IDEA Files

*.iml
*.ipr
*.iws
*.idea

.vscode/
README.html
```

## git and GitHub exercise (individual exercise)

- cd to project directory
- create **.gitignore** file in the project root with the following content below
- type **git init**
- type **git add .**
- type **git commit -m "initial commit"**

- create a new repo in GitHub giving a same name of your project - do not create README.md
- cd to project directory
- type **git remote add origin \<url of the GitHub repo\>**
- type **git push -u origin main** 

## git and GitHub exercise (Group exercise)

- Choose one person in your group as project-leader
- THe project-leader add other team members as collaborators
- The collaborators accept the collaborator invitation
- The collaborators clone the project-leader's project
- Start collaboration

## IntelliJ Shortcut keys

### IntelliJ Shortcut keys for Mac:

- Run app and test
  - CTRL+SHIFT+R (run the app/test)
  - CTRL+R(rerun the app/test)
- Editing
  - CMD+B (go to the source code of a class or method)
  - ALT+Return (Quick fix for compiler error)
  - CMD+SHIFT+Return (Complete current statement)
  - CMD+N (Generate)
  - SHIFT+F6 (Rename)
  - CMD+ALT+V (extract return value into a local variable)
  - F2, SHIFT+F2 (Go to next/previous error)
  - CMD+Left (navigate back)
  - CMD+Right (navigate forward)
- Window management
  - CMD+SHIFT+F12 (maximize/minimize editor window)
  - CMD+SHIFT+' (Maximize/minimize tool window)
- Testing
  - CMD+SHIFT+T (go to target/test code)
- File search
  - CMD+O (find class)
  - CMD+SHIFT+O (find file)
- String search
  - CMD+F (search within a file)
  - CMD+SHIFT+F (search within the project)

### IntelliJ Shortcut keys for Windows:

- Run app and test
  - CTRL+SHIFT+F10 (run the app/test)
  - SHIFT+F5 (rerun the app/test)
  - SHIFT+F10 (rebuild/rerun)
- Editing
  - CTRL+B (go to the source code of a class or method)
  - ALT+Enter (quick fix for compiler error)
  - CTRL+SHIFT+Enter (complete current statement)
  - Alt+Ins (generate)
  - Shift+F6 (rename all instances of a variable)
  - CTRL+ALT+V (extract return value into a local variable)
  - F2, SHIFT+F2 (go to next/previous error)
  - Alt+Left (navigate back between classes)
  - Alt+Right (navigate forward between classes)
- Window management
  - CTRL+SHIFT+F12 (maximize/minimize editor window)
  - CTRL+SHIFT+F12 (maximize/minimize tool window)
  - Alt+F12 (open/close terminal window)
- Testing
  - CTRL+SHIFT+T (go to target/test code)
- File search
  - CTRL+N (find class)
  - CTRL+SHIFT+F (find file)

- [IntelliJ shortcut keys cheat sheet](https://www.jrebel.com/blog/intellij-shortcuts)

### How to enable function keys for certain apps in Mac

- [How to enable function keys for certain apps in Mac](https://www.techrepublic.com/article/how-to-permanently-display-the-function-keys-for-certain-apps-in-the-macbook-pro-touch-bar/)

# Day 2

## DS&A lab projects and IntelliJ

- How to open lab modules
  1. File->Open
  2. Choose "./workspace/dsa-labs" directory
  3. Then you will see all lab modules are displayed

- How to add a new module
  1. File->New->Module
  2. Set the "Name" field to project name of your choice, i.e. "my-project"
  3. Make sure the "Location "field is set to "./workspace/dsa-labs/my-project"

## Binary and Octal Conversion

- Decimal number system

```
Possible numbers: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
decimal 324 = 3 * 100 + 2 * 10 + 4 * 1
decimal 902 = 9 * 100 + 0 * 10 + 2 * 1
```

- Binary number system

```
Possible numbers: 0, 1
binary  101 =         1 * 4 + 0 * 2 + 1 * 1 = decimal value 5
binary 1011 = 1 * 8 + 0 * 4 + 1 * 2 + 1 * 1 = decimal value 11
```

- Octal number system

```
Possible numbers: 0,1,2,3,4,5,6,7
octal  10 =          1 * 8 + 0 * 1 = decimal value 8
octal  17 =          1 * 8 + 7 * 1 = decimal value 15
octal 217 = 2 * 64 + 1 * 8 + 7 * 1 = decimal value 143
```

- Hexadecimal number system

```
Possible numbers: 0,1,2,3,4,5,6,7,8,9,A,B,C,D,E,F
A = decimal 10
B = decimal 11
C = decimal 12
D = decimal 13
E = decimal 14
F = decimal 15
hexadecimal 1A = 1 * 16 + A * 1 = decimal value 26
hexadecimal 1F = 1 * 16 + F * 1 = decimal value 31
```

## Challenge exercise of number string conversion to decimal value

- Write generic conversion code that handles all number systems:
  - binary
  - octal
  - decimal
  - hex-decimal

```java
// "numberBase" argument could be 2,8,10,16 to represent
// binary, octal, decimal, and hexa-decimal respectively
public static int convertFromGeneral(String toBeConverted, 
                                     int numberBase) {

    int decimalValueResult = 0;
    
    //
    // TODO: write your code here
    //
    
    return decimalValueResult;
}
```

## Testing negative cases

- Two different ways of testing if your code generates an exception correctly

```java
// This one just test if InvalidParameterException is thrown
@Test(expected = InvalidParameterException.class)
public void _convertFromOctal_should_throw_InvalidParameterException_given_octal_string_with_non_number_chars() throws InvalidParameterException {
    BinaryConvert.convertFromOctal("17a");
}

// This one also test if the exception message is correct as well
@Test
public void _convertFromOctal_should_throw_InvalidParameterException_given_octal_string_with_non_number_chars2() {
    String badOctalStr = "17a";
    try {
        BinaryConvert.convertFromOctal(badOctalStr);
        fail("Didn't throw exception");
    } catch (InvalidParameterException ipe) {
        assertEquals(badOctalStr, ipe.getMessage());
    }
}
```

- Example custom exception class

```java
public class MyNumberFormatException extends RuntimeException {

    public MyNumberFormatException(String message) {
        super(message);
    }
}
```

- [Number system youtube intro - watch the first ~4 minutes](https://www.youtube.com/watch?v=FFDMzbrEXaE&ab_channel=TheOrganicChemistryTutor)

- ["int" value range - see under "Numbers" section](https://www.i-programmer.info/ebooks/modern-java/5423-java-data-types-numeric-data.html#:~:text=128%20to%20127-,short%202%20bytes%20%2D32%2C768%20to%2032%2C767,4%20bytes%207%20decimal%20digits) 


## Runtime complexity and Big O notation

- Big O rules
  - Different steps get added
  - Drop constants
  - Dominant wins
    - O(n + n<sup>2</sup>) => O(n<sup></sup>)


- [Big O notation Youtube video ~9 minutes](https://www.youtube.com/watch?v=v4cd1O4zkGw&ab_channel=HackerRank)
  

## Runtime complexity of Lab 1.4 - find intersected numbers

- Runtime complexity of neither arrays sorted
  - "O(n square of 2)" worst
- Runtime complexity of one array sorted while the other array is not sorted 
  - "O(n log n) + O(n log n) -> O (n log n)"
  - The first "O(n log n)" is for merge-sorting one array
  - The second "O(n log n)" is for binary searching for "n" items in the other array
- Runtime complexity of both arrays are sorted
  - "2 * O(n log n) + O(n) -> 2 * O(n log n) -> O(n log n)"
  - The first "2 * O(n log n)" is for merge-sorting two arrays
  - The "O(n)" is going through "n" items in one array

## Quick Quiz after Day 2

1. What does O(n) runtime complexity mean?
1. What is the runtime complexity of bubble sort in the form of Big O notation?
1. What is the runtime complexity of binary search in the form of Big O notation?
1. What does "base case" or "base condition" mean in the recursive programming?
1. If you call a method in recursive fashion without "base condition" check, what would happen?
1. Can you explain how QuickSort works at the high level?
1. What are the differences between Checked Exception vs Unchecked exception?
1. What is the top-level Unchecked exception in Java?

# Day 3

## Sorting related resources

- [Animated sorting](https://visualgo.net/en/sorting)

## Bubble sort

- logic of bubble sort

```
- initial array
15, 7, 12, 4, 17, 9, 5, 6

- first iteration k=1
7, 12, 4, 15, 9, 5, 6, [17]
- 2nd  iteration k=2
7, 4, 12, 9, 5, 6, [15, 17]
- 3rd iteration k=3
4, 7, 9, 5, 6, [12, 15, 17]

```

## Binary Search

- Assumed the numbers are already sorted
- Example

```
sorted array: [1, 2, 3, 4, 7, 8, 9, 11, 14, 17, 20]
target: 4

- 1st phase [1, 2, 3, 4, 7]
- 2nd phase [3, 4, 7]
- 3rd phase [4]
```

## Steps of recursive programs

Every recursive program follows the same basic sequence of steps:

1. Initialize the algorithm. Recursive programs often need a seed value to start with. This is accomplished either by using a parameter passed to the function or by providing a gateway function that is non-recursive but that sets up the seed values for the recursive calculation.
2. **Check to see whether the current value(s) being processed match the base case.** If so, process and return the value.
3. Redefine the answer in terms of a smaller or simpler sub-problem or sub-problems.
4. Run the algorithm on the sub-problem.
5. Combine the results in the formulation of the answer.
6. Return the results.

## Quick sort resources

- [Quicksort: Partion'ing an array (~5 minutes)](https://www.youtube.com/watch?v=MZaf_9IZCrc&ab_channel=KCAng)
- [Lomundo quicksort youtube video (~3 minutes)](https://www.youtube.com/watch?v=86WSheyr8cM&ab_channel=BukanCaraCepat)


## Challenge/Quiz questions after Day 3

- What is the "base case"/"base condition" of the quick sort?
- Is it possible to support Queue operations of "enqueue() to the tail" and "dequeue() from head" with a singular link node (instead of double link node as we've seen in our lab) assuming the queue has still both "head" and "tail"? 
- In the "pop" operation in the stack below, do we have to do any extra null pointer check of the "node.next" on the line of "head = node.next"?  In other words, can we set the head with "null"?

```
// pseudo code
item pop( )
    if (head != null)
        node = head
        head = node.next 
        return node.value
    return null
```

# Day 4

## Linked List resources

- [Picture of linked list](https://www.geeksforgeeks.org/difference-between-singly-linked-list-and-doubly-linked-list/)

## Simple binary tree sample example

- [Binary Tree with numbers](https://www.baeldung.com/java-binary-tree)

# Day 5
  
## Dependency Injection Demo

- [Sang Shin's Dependency Injection Youtube demo](https://www.youtube.com/watch?v=kmQiiT4pATo&ab_channel=SangShin)

## Java Lambda, Functional Interface, Java Streams presentations

- [Lambda syntax presentation slides](https://github.com/sashinpivotal/java-presentations/blob/main/javase8_lambda_syntax.pdf)
- [Functional Interface presentation slides](https://github.com/sashinpivotal/java-presentations/blob/main/javase8_lambda_fi.pdf)
- [Java Streams presentation slides](https://github.com/sashinpivotal/java-presentations/blob/main/javase8_lambda_streams.pdf)

## How to add logging to your Maven project

1. Add dependencies below to your *pom.xml". 
   Make sure you click "Maven refresh" icon in your IntelliJ

```xml
        <!-- https://mvnrepository.com/artifact/org.slf4j/slf4j-api -->
        <dependency>
            <groupId>org.slf4j</groupId>
            <artifactId>slf4j-api</artifactId>
            <version>1.7.36</version>
        </dependency>
        <!-- https://mvnrepository.com/artifact/org.slf4j/slf4j-simple -->
        <dependency>
            <groupId>org.slf4j</groupId>
            <artifactId>slf4j-simple</artifactId>
            <version>1.7.36</version>
        </dependency>
```

2. Create "resources" directory under "src/main"
3. Create *logback.xml* under "src/main/resources" directory
   with the following contents

  ```xml
  <configuration>
      <appender name="STDOUT" class="ch.qos.logback.core.ConsoleAppender">
          <encoder>
              <pattern>%d{HH:mm:ss.SSS} [%thread] %-5level %logger{36} - %msg%n</pattern>
          </encoder>
      </appender>

      <root level="debug">
          <appender-ref ref="STDOUT" />
      </root>
  </configuration>
  ```

4. Add the following code to your class as a field and 
   import classes

```java
private static final Logger logger
        = LoggerFactory.getLogger(HRClient.class);
```

5. Add the following code for actually logging

```java
logger.info("----------- logger info message");
```

6. Run the application and observe the logging messages
