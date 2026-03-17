# 🔁 Types of Recursion: Head Recursion in Python

## 🎯 AIM:
To write a Python program to display Arithmetic Progression  series by reading the difference between the numbers and limit  using  head recursion.

## 🧠 ALGORITHM:

1. Start the function fun(n, d).
2. If n is greater than 0, proceed; otherwise, stop.
3. Call fun(n - d, d) to recursively reduce n by d.
4. After the recursive call finishes, print the current value of n on the same line.
5. Read inputs d (step value) and x (starting number).
6. Call fun(x, d) to display numbers from smallest positive step up to x.

## 💻 PROGRAM:
~~~
def fun(n,d):
    if (n > 0):
        fun(n - d,d)
        print(n, end=" ")
 
d= int(input())
x = int(input())
fun(x,d)

~~~

## OUTPUT
<img width="1254" height="256" alt="image" src="https://github.com/user-attachments/assets/c49e26d9-1851-4c1a-a8c8-758fd3182596" />



## RESULT
Thus the required head recursion ouput is Verified.
# 🔁 Recursion:nested Recursion in Python

## 🎯 AIM:
To write a Python program to display all the positive numbers in reverse order with a difference 2 from 'N'  using nested recursion

---

## 🧠 ALGORITHM:

1. Start the function fun(n).
2. If n equals 1, return 1.
3. If n equals 0, return 0.
4. Otherwise, print the current value of n without moving to the next line.
5. Call fun(n - 2) and pass its result again into fun().
6. Output the final returned value from the nested recursive calls.
---

## 💻 PROGRAM:
~~~
def fun(n):
    if n==1:
        return 1
    elif n==0:
        return 0
    else:
        print(n,end=" ")
        return(fun(fun(n-2)))
        
n=int(input())
print(fun(n))
~~~

## OUTPUT
<img width="356" height="166" alt="image" src="https://github.com/user-attachments/assets/ef975f79-7672-4d3f-b99f-2364fdcfeb64" />

## RESULT
Thus the Nested recursion is verified.
# # 🔁 Recursion:Sum of Digits using Recursion in Python

## 🎯 AIM:
To write a Python program to calculate the **sum of all digits** in a number using **recursion**.

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `sum_digit(n)` that:
   - Returns 0 if `n <= 0` (Base Case)
   - Else, returns `n % 10 + sum_digit(n // 10)` (Recursive Case)
3. Take integer input from the user.
4. Call the recursive function and store the result.
5. Print the result.
6. **Stop**

## 💻 PROGRAM:
~~~
def sum_digit(num):
    if num < 0 or int(num) != num:
        return 0
    elif num == 0:
        return 0
    else:
        return (num % 10) + sum_digit(num//10)
num= int(input())
print(sum_digit(num))
~~~

## OUTPUT
<img width="467" height="220" alt="Screenshot 2025-09-08 085403" src="https://github.com/user-attachments/assets/6966fc70-cf5d-4722-8f75-20cf7a6682cb" />


## RESULT
Thus the output is verified.
# 📐 Taylor Series Using Recursion in Python

## 🎯 AIM:
To write a Python program to evaluate a **Taylor Series** using **recursion**, where values of `x` and `n` are taken from the user.

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `x` and `n`
3. Get values for `x` and `n` from the user
4. Define a recursive function `series(x, n)`
   - **Base case:** If `n == 0`, return 1
   - **Recursive case:** Return `x**n / n + series(x, n-1)`
5. Print the result
6. **Stop**

## 💻 PROGRAM:
```
def fun(x,n):
    if(n==0):
        return 1 
    else:
        return ((2**n)*(x**n)+fun(x,n-1))
x=int(input())
n=int(input())
print(fun(x,n))
```
## OUTPUT
<img width="390" height="230" alt="image" src="https://github.com/user-attachments/assets/47cda7a1-6e33-4a39-be6f-1f9f2d152683" />

## RESULT
Thus the output is verified.
# 📐 Taylor Series:sinh(x) Evaluation using Recursion in Python

## 🎯 AIM:
To write a Python program to evaluate the value of **sinh(x)** for **n terms** using recursion.

---

## 🧠 ALGORITHM:

1. **Start**
2. Read input for variable `x` (angle or number)
3. Read input for variable `n` (number of terms)
4. Define a function `fact(n)`:
   - If `n <= 1`, return 1
   - Else, return `n * fact(n - 1)` (recursive factorial)
5. Define a function `sinh(x, n)`:
   - If `n == 0`, return `x`
   - Else, return `(pow(x, 2*n + 1) / fact(2*n + 1)) + sinh(x, n - 1)`
6. Call the `sinh(x, n)` function and print the result
7. **Stop**

---

## 💻 PROGRAM:
~~~
def fact(i):
    if i==0 or i==1:
        return 1
    else:
        return i*fact(i-1)
def sine(x,n):
    if n==0:
        return x
    else:
        return pow(x,(2*n+1))/(fact(2*n+1))+sine(x,n-1)
x=int(input())
n=int(input())
print(sine(x,n))
~~~


## OUTPUT
<img width="550" height="225" alt="image" src="https://github.com/user-attachments/assets/eb2d8220-487d-4752-9657-c21830280ea6" />



## RESULT
Thus the required output is got and verified.
