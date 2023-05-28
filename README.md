<img src="https://static.vecteezy.com/system/resources/previews/019/899/953/non_2x/java-free-download-free-png.png" alt="Logo" width="200" height="200">

# Java Recursion Exercises.

A set of recursion exercises in java, algorithm explanation, tips, tracks and solutions. 

## Installation

In order to test the code, just download the Main.java file and run:

```bash
  javac Main.java
  java Main
```

## Introduction to Recursive Algorithms.

In this repository, you will find a collection of recursive algorithms explained and demonstrated. If you're new to recursion or want to reinforce your understanding, I recommend watching this informative video: https://www.youtube.com/watch?v=70ESDR5YQtY

The video beautifully illustrates the concept of recursion using a set of bricks arranged in a domino effect. Each brick pushes the next one, creating a cascading effect until the final brick is accommodated. Once the last brick is in place, the process starts again, but in reverse, until it reaches the very first brick. This looping pattern reflects the essence of recursion.

**Understanding Recusion in Code:**  Now that we have a general understanding of recursion, let's explore how it works in code. We'll use the bricks video as an example.

```java
void arrangeBricks(Brick[] bricks) {
  if (Is there a brick next to me?) {
    pushBrick(current brick);
    return arrangeBricks(nextBrick);
    acommodateBrick();
  } else {
    return; // No more bricks! Let's exit the function.
  }
}
```
Here, we have a function called arrangeBricks that takes an array of bricks as input. The initial if statement checks if there is another brick next to the current one. If so, it pushes the next brick and recursively calls arrangeBricks with the next brick as an argument. Note that each recursive call waits for the subsequent call to return the pushed brick to accommodate it. In case there are no more bricks, the function simply exits.

Recursion allows us to create loops by calling the same function repeatedly. Each iteration waits for the recursive function to return a value or perform an action, allowing us to utilize the returned value effectively.

Now that we have a better understanding of recursive algorithms, let's dive into the exercises included in this repository and further enhance our skills.

## Excercises, Tips, Clues and Solutions.

 - **Factorial:**

A factorial number is a mathematical concept that represents the multiplication of all positive integers from 1 to a given number. It is denoted using the exclamation mark symbol (!). For example, the factorial of 5 is written as 5! and is calculated by multiplying 5 by 4, then by 3, then by 2, and finally by 1, resulting in 120. Factorial numbers are used in various areas of mathematics and statistics, as well as in recursive algorithms and combinatorics.

**Excersise:** Given n of 1 or more, return the factorial of n, which is n * (n-1) * (n-2) ... 1. Compute the result recursively (without loops).

**Clue:** The secret to resolve this algorithm is by looking at the formula. 

**Tip:** Remember that we need to get focused on what the function will return in the future and then operate the value.

**Solution:**


 ```java
public int factorial(int n) {
  if(n==1) return 1;
  
  return n * factorial(n-1);
}

```

**Explanation:**
<img src="graphicexamples/factorial.png">


