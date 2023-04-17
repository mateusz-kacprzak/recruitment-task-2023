# Recruitment task 2023 :duck:
## Goal
Your task is to implement a program that retrieves numbers via the REST service and picks only prime numbers. It must continue until ***20 distinct prime numbers*** are collected.
Once this is done, the following information must be provided to the end-user:

1. List of the collected prime numbers.
2. Count of REST api calls.
3. Total count of all numbers processed.


Style of presentation depends on you. Console interface is a minimum, whereas eye-catching graphical presentation (application/web page) is a plus.


Note that it must be easy to trigger the program again. It could be by pressing a key or clicking a button.
### Resources

- The API URL: http://www.randomnumberapi.com/api/v1.0/random?min=1&max=1000&count=100
- API returns an array of at most 100 random numbers between [min,max]
  - np.     ```
    [898, 376, 189, 3, 759, 555, 388, 491, 286, 649, 416, 242, 223, 409, 104, 84, 563, 190, 69, 935, 809, 376, 966, 423, 297, 577, 739, 624, 345, 276, 854, 304, 477, 707, 657, 564, 851, 994, 844, 533, 773, 467, 408, 237, 372, 376, 439, 513, 23, 907, 271, 985, 669, 393, 552, 200, 324, 947, 543, 419, 89, 67, 905, 686, 120, 197, 310, 872, 325, 405, 969, 864, 497, 332, 195, 146, 787, 629, 258, 402, 775, 279, 963, 392, 226, 991, 932, 721, 472, 768, 870, 184, 987, 188, 191, 189, 635, 874, 264, 786]     ```
- You can freely modify min(>=0) and max(<10000) parameters 
- read more https://www.randomnumberapi.com/ in ***Get a random number*** section

If there are any problems with the API then please email me at mateusz.kacprzak@dynatrace.com

## Example
Launching
```
java -jar task.jar
```
```
===Hello===.
Do you want to start gathering numbers?
Yes
```
Program result in the console
```
===Result===
Number of requests to external service: 4
Number of numbers processed: 400
Prime numbers after filtering: [2, 3, 5, 7, 11, 13, 17, 19, 179, 181, 191, 193, 197, 239, 241, 251, 257, 389, 727, 2137].
===End of the result===.

Do you want to run another retrieval?
Yes

===Result===
Number of requests to external service: 5
Number of numbers processed: 500
Prime numbers after filtering: [7, 11, 13, 17, 19, 179, 181, 191, 193, 197, 239, 241, 251, 257, 389, 727, 733, 1087, 1091, 2137].
===End of the result===

Do you want to run another retrieval?
No
===Bye===
```

### Requirements
- Duplicates are not allowed in the prime number collection
- Prime number collection must be sorted
- It must be easy to trigger the program again

### Technical requirements
- The main part of the application must be implemented in Java
- The presentation part can be implemented in any technology
- The solution must be in a GitHub repository. The access to the repository must be granted to user https://github.com/mateusz-kacprzak
- You need to create a README file with the application description and the way to launch it

### Dos and don’ts
- It is allowed to use any Java framework
- You can write the frontend application in any technology/framework to present the result (it will even be extra plus)
- The result can even be presented in the console
