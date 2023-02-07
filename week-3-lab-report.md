# **Week 3 Lab Report - Skyler Nguyen**

## Servers and Bugs

## Part 1

* Code for StringServer

<img width="509" alt="image" src="https://user-images.githubusercontent.com/122576334/215218619-6f594c17-be54-4aa7-a522-560d4568e1de.png">
<img width="583" alt="image" src="https://user-images.githubusercontent.com/122576334/215218826-653fd00e-9f5d-445f-a602-8863513ce81c.png">

* Screenshots of /add-message

<img width="284" alt="image" src="https://user-images.githubusercontent.com/122576334/215219046-7f3aa4b3-d537-41d7-9731-3b15e6b60300.png">

  <img width="353" alt="image" src="https://user-images.githubusercontent.com/122576334/215219079-d698c7fd-8478-4b84-b923-88dd0e075159.png">

* The methods 'main' and 'handleRequest' are called in both screenshots. 'main' starts a server using a port number when running StringServer.java. 'handleRequest' takes the argument url and prints out the field 'messages' onto the server.
* The relevant arguments to those methods are the user's port number and the url of the server. The value of the field 'messages' changes everytime the user reloads the server or changes the url after '/add-message?s='. This is done by the 'handleRequest' method getting the path of the field (using getPath) 'url' which is just the url of the server and then checks if it has /add-message' in it. If it does, the values of the field 'parameters' is set using getQuery.split("=") which takes in everything after the question mark and then sets index 0 of 'parameters' the element to the left side of the equal sign and index 1 of 'parameters' the element to the right side of the the equal sign. Lastly, the method checks if index 0 of 'parameters' is 's' and if it is, adds the element of index 1 of 'parameters'.
* The value of messages gets changed everytime the server is ran and there is a message to add.

## Part 2

* The bugged method is reversed.

* Failure-inducing input:
```
  @Test 
  public void testBugReversed() {
    int[] input = {0, 1};
    assertArrayEquals(new int[]{1, 0}, ArrayExamples.reversed(input));
  }
```

* An input that doesn't induce a failure:
```
  @Test 
  public void testBugReversed2() {
    int[] input = {0};
    assertArrayEquals(new int[]{0}, ArrayExamples.reversed(input));
  }
```

* The symptom:

  <img width="742" alt="image" src="https://user-images.githubusercontent.com/122576334/215243565-d67d8f84-f4ae-42e8-9b88-8a87d2e57e93.png">

* The bug before:
```
  static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
```

* The bug after:
```
  static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  }
```

* The fix addressed the issue because the for loop was trying to change the elements of the old array with elements with the new array but the new array has no elements in it so it changed the old array into {0, 0}. Additionally, we want to return the new array with the reversed elements, not the old one.

## Part 3

* Something I learned in Week 2 that I didn't know before was that you can create and start your own server using VSCode. In CSE 11, we only learned the basics of java and didn't get into any other things. Thus, learning that you can start a server was cool.


