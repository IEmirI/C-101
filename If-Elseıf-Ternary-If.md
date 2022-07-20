# C#-101
# If-ElseIf-Ternary-If
## Objective
### In this challenge, we learn about conditional statements. Check out the Tutorial tab for learning materials and an instructional video.

## Task

### Given an integer,n, perform the following conditional actions:
### If n is odd, print Weird
### If n is even and in the inclusive range of 2 to 5, print Not Weird
### If n is even and in the inclusive range of 6 to 20, print Weird
### If n is even and greater than 20, print Not Weird
### Complete the stub code provided in your editor to print whether or not n is weird.

## Input Format

### A single line containing a positive integer, n.

## Constraints

```
1 <= N <= 100
```

## Output Format

### Print Weird if the number is weird; otherwise, print Not Weird.

## Sample Input 0
```
3
```
## Sample Output 0
```
Weird
```
## Sample Input 1
```
24
```
## Sample Output 1
```
Not Weird
```
## Explanation

### Sample Case 0: n = 3
### n is odd and odd numbers are weird, so we print Weird.

### Sample Case 1: n = 24
### n > 20 and n is even, so it is not weird. Thus, we print Not Weird.

```
class Solution
{
    public static void Main(string[] args)
    {
        int N = Convert.ToInt32(Console.ReadLine().Trim());
        if (1 <= N && N <= 100)
        {
            if ((2 <= N) && (N <= 5))
            {
                if (N % 2 == 1)
                { Console.WriteLine("Weird"); }
                else { Console.WriteLine("Not Weird"); }
            }
            else if (6 <= N && N <= 20)
            {
                if (N % 2 == 1)
                { Console.WriteLine("Not Weird"); }
                else { Console.WriteLine("Weird"); }
            }
            else if (20 < N)
            {
                if (N % 2 == 1)
                { Console.WriteLine("Weird"); }
                else { Console.WriteLine("Not Weird"); }
            }
        }
    }
}

```

# [Patika.dev](https://app.patika.dev/courses/csharp-101/1-if-else-yapisi-ve-ternary-if)