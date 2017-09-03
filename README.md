# Ninja Finder Challenge

## Requirements

Design and deploy an API endpoint that will provide the 4 methods described below.

- The API must be **deployed** in your favorite Cloud provider.
- Methods will be called by a test case suite to validate their correctness.
- Inputs/outputs must respect the proposed JSON structure.

## Advice

- The goal here is not to absolutely get a good answer. We want to see your approach to problem solving. We will ask you thereafter to explain to us why you choose to solve the problem the way you did. So, make the code reflect how you actually write code in real life. Including naming, flow, structure, error handling, etc. For instance, you can create as many sub methods as necessary. 
- Your code should be able to handle just about anything thrown at it without raising an Exception. If something is not stated in the problem, assume the worst and code around it.
- Ensure that your code is properly tested

## Questions
### Problem 1 - Unique Values

Provide a **POST** method at **/uniquevalues** that returns true if all the input values are distinct.

**Input**: An array of N items.

**Output**: true if all the input values are distinct or if the array is empty or if the array is null. False otherwise.

Example 1 : [1] returns true.

Example 2 : [1, 3, 1] returns false.

Example input format:

```json
{
    "input": [1, 3, 1]
}
``` 
Example output format:

```json
{
  "result": true
}
``` 

### Problem 2 - Permutations

Provide a **POST** method at **/permutations** that generates all the possible permutations from a set of integers provided as a String. For instance, given the String "1 3", the method should return "1 3" and "3 1" as a list of strings.

**Input**: A string of positive integers. The integers in the input strings will be separated by one or more spaces. The input may contain duplicate elements.

**Output**: An instance of java.util.List<String>, containing a distinct set of permutations. Each integer should be separated by a single space. The Strings should be trimmed.

Example : "1 3" will return ["1 3", "3 1"].

Example input format:

```json
{
    "input": "1 2"
}
``` 

Example output format:

```json
{
  "result": [
    "2 1",
    "1 2"
  ]
}
``` 

### Problem 3 - Reverse

Provide a **POST** method at **/reverse** that returns the provided integers in reverse order.

**Input**: A string of positive integers. The integers in the input string will be separated by one or more spaces. The input may contain duplicate elements.

**Output**: The reverse version of the input string. Each integer should be separated by a single space. The string should be trimmed.

Example : "1   2 3  " should return "3 2 1"

Example input format:

```json
{
    "input": "1 2"
}
``` 

Example output format:

```json
{
  "result": "2 1"
}
``` 

### Problem 4 - Prime Palindrome

Provide a **GET** method at **/primepalindrome** that returns the biggest prime number, which is also a palindrome, within the range of 1 - 1000. This being a constant, a good coder would just return the hard coded value. But, in the spirit of this test, please provide a complete solution to programmatically find the answer.

**Input**: none.

**Output**: An integer that meets the problem statement.

Example output format:

```json
{
  "result": 1000
}
``` 
