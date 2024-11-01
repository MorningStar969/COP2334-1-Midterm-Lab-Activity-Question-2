# COP2334-1-Midterm-Lab-Activity-Question-2
This is a GitHub repository link for the answer to question 2 of the midterm lab activities

// This program is used to determine how many even and odd numbers the user has entered and if they are divisible by 2.

// Include the iostream library
#include <iostream>
using namespace std; // Using standard namespace

// Main function
int CountEvens(int num1, int num2, int num3, int num4, int num5) {
   int count = 0; // Initialize count to 0
   if (num1 % 2 == 0) ++count; // If num1 is even, increment count
   if (num2 % 2 == 0) ++count; // If num2 is even, increment count
   if (num3 % 2 == 0) ++count; // If num3 is even, increment count
   if (num4 % 2 == 0) ++count; // If num4 is even, increment count
   if (num5 % 2 == 0) ++count; // If num5 is even, increment count
   return count; // Return count
}

// Main function
int CountOdds(int num1, int num2, int num3, int num4, int num5) {
   int count = 0; // Initialize count to 0
   if (num1 % 2 != 0) ++count; // If num1 is odd, increment count
   if (num2 % 2 != 0) ++count; // If num2 is odd, increment count
   if (num3 % 2 != 0) ++count; // If num3 is odd, increment count
   if (num4 % 2 != 0) ++count; // If num4 is odd, increment count
   if (num5 % 2 != 0) ++count; // If num5 is odd, increment count
   return count; // Return count
}

// Main function
int main() {
   cout << "Enter five numbers: "; // Prompt the user to enter five numbers
   int num1, num2, num3, num4, num5; // Declare five integer variables
   cin >> num1 >> num2 >> num3 >> num4 >> num5; // Read five numbers from the user
   cout << "Number of evens: " << CountEvens(num1, num2, num3, num4, num5) << endl; // Print the number of evens
   cout << "Number of odds: " << CountOdds(num1, num2, num3, num4, num5) << endl; // Print the number of odds
   return 0; // Return 0 to indicate successful execution
}
