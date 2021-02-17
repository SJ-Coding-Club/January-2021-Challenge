# Challenge 01
This one is designed to be more beginner friendly. If you're confused on how to do something, just ask me!

You can earn points by submitting solutions for any of the problems, so don't worry about finishing all of them if you can't yet.

<b>Please</b> create a separate file for each problem you submit to Google Classroom.

## Leaderboard

| Contestant | Problem 00| Problem 01| Problem 02| Problem 03| Problem 04|
|-|-|-|-|-|-|
| Jack Donofrio | N/A | N/A | N/A | N/A | N/A |
| Jon Jazwinski | 1/1 | 2/2 | N/A | N/A | N/A |
| Samir Rajani | 1/1 | 2/2 | 3/3 | 4/4 | 4/5 |

## Problem 00
Write a program that prints "My first submission!" to standard output.

## Problem 01
Write a program that prints "Hello, {name}!" where {name} is your name. 
- Example: "Hello, Jack!"

## Problem 02
Write a program that calculates the volume of a cone with a radius of 5 and a height of 9.

## Problem 03
Write a program that converts 40 degrees Celsius to degrees Fahrenheit. 
<details>
<summary>Hint </summary>
F = C * 9/5 + 32
</details>

## Problem 04
Write a program that computes the roots of <b>x<sup>2</sup> + 16x + 52 = 0</b>.
<details>
  <summary>Hint 1</summary>
   Two rational roots exist.
</details>
<details>
  <summary>Hint 2</summary>
  The quadratic equation might help
</details>
<details>
  <summary>Hint 3</summary>
  https://imgur.com/pjyy2l6
</details>

# Solutions

## problem00.py
``` Python
print("My first submission!")
```

## problem01.py
Suitable:
``` Python
print("Hello, Jack!")
```
But this is better:
``` Python
name = "Jack"
print(f"Hello, {name}!")
```

## problem02.py
``` Python
PI = 3.14159
radius = 5
height = 9
volume = 1 / 3 * radius * radius * height * PI
print(volume)
```
or
``` Python
import math
radius = 5
height = 9
volume = 1 / 3 * pow(radius, 2) * height * math.pi
print(f"volume = {volume}")
```

## problem03.py
``` Python
c = 40
f = c * 9/5 + 32
print(f"{c} degrees Celsius is {f} degrees Fahrenheit")
```

## problem04.py
``` Python
import math
# x^2 + 16x + 52 = 0
# a^2 + bx + c form
a = 1
b = 16
c = 52
root_1 = (-b + math.sqrt(b*b - 4*a*c)) / (2*a)
root_2 = (-b - math.sqrt(b*b - 4*a*c)) / (2*a)
print(root_1, root_2)
```
Alternatively
``` Python
import math
a = 1
b = 16
c = 52
discriminant = b*b - 4*a*c
root_1 = (-b + math.sqrt(discriminant)) / (2*a)
root_2 = (-b - math.sqrt(discriminant)) / (2*a)
print(root_1,root_2)
```
