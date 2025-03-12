# least-number

## student info
-Name: robel wondwesen 
-ID number: 0752/23
-course: DSA
## algorthm
Algorithm to Find Second and Third Largest Numbers
Input Phase:
Prompt the user to enter the number of elements, n.
Initialize an empty list (or vector) to store n integers.
Loop n times:
Read an integer from the user and append it to the list.
Function to Find Second Largest:
Initialize two variables:
first to the minimum possible integer value (using numeric_limits<int>::min()).
second to the minimum possible integer value.
Loop through each number in the array:
If the current number is greater than first:
Assign the value of first to second.
Update first to the current number.
Else if the current number is greater than second and not equal to first:
Update second to the current number.
After the loop, check if second is still the minimum integer value:
If yes, return -1 (indicating no second largest exists).
Otherwise, return second.
Function to Find Third Largest:
Initialize three variables:
first, second, and third to the minimum possible integer value.
Loop through each number in the array:
If the current number is greater than first:
Assign the value of second to third.
Assign the value of first to second.
Update first to the current number.
Else if the current number is greater than second and not equal to first:
Assign the value of second to third.
Update second to the current number.
Else if the current number is greater than third, not equal to first, and not equal to second:
Update third to the current number.
After the loop, check if third is still the minimum integer value:
If yes, return -1 (indicating no third largest exists).
Otherwise, return third.
Main Function Logic:
Prompt the user to choose whether to find the second or third largest number.
Depending on the user's choice:
Call findSecondLargest() and display the result.
Call findThirdLargest() and display the result.
Handle invalid choices by displaying an error message.
