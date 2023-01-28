# **Week 3 Lab Report - Skyler Nguyen**

## Servers and Bugs

## Part 1

* Code for StringServer

<img width="509" alt="image" src="https://user-images.githubusercontent.com/122576334/215218619-6f594c17-be54-4aa7-a522-560d4568e1de.png">
<img width="583" alt="image" src="https://user-images.githubusercontent.com/122576334/215218826-653fd00e-9f5d-445f-a602-8863513ce81c.png">

* Screenshots of /add-message

<img width="284" alt="image" src="https://user-images.githubusercontent.com/122576334/215219046-7f3aa4b3-d537-41d7-9731-3b15e6b60300.png">
<img width="353" alt="image" src="https://user-images.githubusercontent.com/122576334/215219079-d698c7fd-8478-4b84-b923-88dd0e075159.png">

* The methods main and handleRequest are called.
* The relevant argument is parameters[1] + "\n" which adds the message to the variable to be printed out. The values of messages are all the strings that are being added.
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


