# **Week 3 Lab Report - Skyler Nguyen**

## Servers and Bugs

## Part 1

* Code for String Server

<img width="509" alt="image" src="https://user-images.githubusercontent.com/122576334/215218619-6f594c17-be54-4aa7-a522-560d4568e1de.png">
<img width="583" alt="image" src="https://user-images.githubusercontent.com/122576334/215218826-653fd00e-9f5d-445f-a602-8863513ce81c.png">

* Screenshot of /add-message

<img width="284" alt="image" src="https://user-images.githubusercontent.com/122576334/215219046-7f3aa4b3-d537-41d7-9731-3b15e6b60300.png">

<img width="353" alt="image" src="https://user-images.githubusercontent.com/122576334/215219079-d698c7fd-8478-4b84-b923-88dd0e075159.png">

* The methods main and handleRequest are called.
* The relevant argument is parameters[1] + "\n" which adds the message to the variable to be printed out. The values of messages are all the strings that are being added.
* The value of messages gets changed everytime the server is ran and there is a message to add.

## Part 2

* The bugged method is reversed.
* Failure-unducing input:
```
  @Test 
  public void testBugReversed() {
    int[] input = {0, 1};
    assertArrayEquals(new int[]{1, 0}, ArrayExamples.reversed(input));
  }
```



