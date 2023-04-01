# Factorial-of-a-Number-in-Java

Factorial of a Number in Java
Here on this page, we will learn how to Find the Factorial of a Number in Java. Factorial is a sequence of a number where we multiply by all previous numbers.

factorial of n (n!) = 1 * 2 * 3 * 4....n


Note : 0! = 1 and 1! = 1

Example : 
5! = 1 * 2 * 3 * 4 * 5 = 120
Factorial of a Number in Java 1

Methods we will discuss
Iterative approach for factorial
Recursive approach for factorial
Method 1
For an input num

Initialize fact = 1
If num < 0 : Print Error as we can’t calculate factorial of a negative number
Else run a iterative loop in iteration of (i) between [1, num]
do fact = fact * i
print the value of fact
Java Code
Run
class Main
{
    // Method to find factorial of the given number
    static int factorial(int n)
    {
        int res = 1, i;
        for (i = 2; i <= n; i++)
            res *= i;
        return res;
    }
    
    // Driver method
    public static void main(String[] args)
    {
        int num = 6;
        System.out.println("Factorial of " + num + " is " + factorial(num));
    }
}
Output:
Factorial of 6 is 720
Method 2
This method uses the recursive approach, for input num

For an input num

Call function getFactorial(num)
Set base case when num== 0 return 1
Other cases return num * getFactorial(num-1);
Java Code
Run
class Main
{
	// method to find factorial of given number
	static int factorial(int n)
	{
		if (n == 0)
			return 1;
		return n * factorial(n - 1);
	}
	
	// Driver method
	public static void main(String[] args)
	{
		int num = 6;
		System.out.println("Factorial of " + num + " is " + factorial(num));
	}
}
Output:
Factorial of 6 is 720
