# HackerRank_solutions

this code contains solutions for - https://www.hackerrank.com/domains/algorithms

    SOLUTIONS IN PYTHON 

        As how the code works :-

1. Equalize the array - https://www.hackerrank.com/challenges/equality-in-a-array/problem?isFullScreen=true

solving method:

->Create an array called "buckets" with a size of 101. This array will be used to count the frequencies of elements in the input array. The size 101 is chosen to accommodate integer values between 0 and 100 (as per the constraints).

->Loop through the elements in the input array "arr" and increment the corresponding bucket in the "buckets" array for each element. This step counts the frequency of each unique element in the input array.

->Calculate the minimum number of deletions needed by subtracting the maximum value in the "buckets" array from the total number of elements in the input array. This step determines the number of deletions needed to leave only elements of equal value.

->The result is written to the output file specified by "os.environ['OUTPUT_PATH']."

2. A very big sum - https://www.hackerrank.com/challenges/a-very-big-sum/problem?isFullScreen=true

solving method:

->The aVeryBigSum function takes a list of long integers (LONG_INTEGER_ARRAY ar) as input and returns their sum as a long integer.

->In the if __name__ == '__main__': block, the program reads the input and writes the output to the specified file, which is determined by the 'OUTPUT_PATH' environment variable.

->The first line inside this block reads an integer ar_count representing the number of elements in the array.

->The second line reads the array elements as a space-separated list of integers and stores them in the list ar.

->The aVeryBigSum function is called with the array ar, and the result is stored in the variable result.

->Finally, the result is written to the output file, and the file is closed.

3. ACM ICPC Team - https://www.hackerrank.com/challenges/acm-icpc-team/problem?isFullScreen=true

solving method:

->The acmTeam function takes a list of binary strings (topic) as input.

->It initializes two variables, most to store the maximum number of topics known and most_cnt to store the count of teams that know the maximum number of topics.

->The function uses two nested loops to compare each pair of attendees' knowledge. It calculates the number of topics known by a team by comparing the binary strings element-wise using a list comprehension and zip. The sum function is used to count the number of '1's in the result.

->If the number of topics known by the current team is greater than the current maximum (most), it updates most to the new maximum and resets the count of teams that know the maximum (most_cnt) to 1. If the number of topics known is equal to the current maximum, it increments the count of teams that know the maximum.

->The function returns a tuple containing the maximum number of topics known (most) and the count of teams that know that many topics (most_cnt).

->In the main part of the code, it reads the input, calls the acmTeam function, and writes the results to the output file as required.

4. Compare the Triplets - https://www.hackerrank.com/challenges/compare-the-triplets/problem?isFullScreen=true

solving method:

->The compareTriplets function takes two lists (a and b) as input, where each list represents the respective ratings of Alice and Bob for three categories.

->It initializes a list res with two elements, both set to 0. These elements will represent Alice's score and Bob's score.

->The function uses a loop to iterate through the elements of the a and b lists simultaneously using the zip function. For each pair of ratings, it compares the values:

* If a[i] is greater than b[i], Alice is awarded a point, so res[0] (Alice's score) is incremented by 1.
* If b[i] is greater than a[i], Bob is awarded a point, so res[1] (Bob's score) is incremented by 1.
  
->The function returns the res list, where the first element represents Alice's score, and the second element represents Bob's score.

->In the main part of the code, it reads the input for Alice's and Bob's ratings, calls the compareTriplets function, and writes the results to the output file as required. The results are printed on the same line, separated by a space.

  5. Organizing Containers of Balls - https://www.hackerrank.com/challenges/organizing-containers-of-balls/problem?isFullScreen=true
 
   solving method:

 ->The organizingContainers function is defined to solve the problem. It takes a 2D array container as input.

  ->It uses two lists, ball_cnt and cc, to keep track of the sum of balls in each container and the count of containers with the same sum, respectively.

   ->It iterates through each container in the input, calculating the sum of balls in each container and updating the ball_cnt and cc lists accordingly.

  ->After processing all containers, the code checks if it's possible to rearrange the balls by comparing the sums of balls in each container (ball_cnt) with the count of containers with the same sum (cc). If all balls can be rearranged as required, it returns "Possible." Otherwise, it returns "Impossible."

  ->In the main part of the code, it reads the input, processes multiple queries, and writes the results to the output file as required.


  6. Plus Minus - https://www.hackerrank.com/challenges/plus-minus/problem?isFullScreen=true

solving method:

->The plusMinus function takes an array arr as input.

->It initializes three variables, p, m, and z, to count the number of positive, negative, and zero elements, respectively.

->It then iterates through the array and updates the counters accordingly.

->After counting, it calculates the ratios by dividing the counts by the total number of elements (n).

->Finally, it prints the ratios with exactly 6 decimal places using formatted strings.

->In the main part of the code, it reads the input, calls the plusMinus function, and prints the results as required.

7.  Queen's Attack II - https://www.hackerrank.com/challenges/queens-attack-2/problem?isFullScreen=true

   solving method:

  -> The queensAttack function takes the board size n, the number of obstacles k, the queen's row position r_q, the queen's column position c_q, and the positions of obstacles in the form of a 2D array.

->The function initializes variables to keep track of the closest obstacles in the left, right, up, down, and diagonal directions.

->It calculates the diagonals (d1_up, d1_down, d2_up, d2_down, d1_q, d2_q, and d_q) that intersect with the queen's position.

->The function iterates through the obstacles, updating the variables based on their positions. For example, it checks if an obstacle is on the same row, column, or diagonal as the queen and updates the variables accordingly.

->Finally, the function calculates the total number of squares the queen can attack by subtracting the limits imposed by the obstacles from the total available squares.

->In the main part of the code, it reads the input, calls the queensAttack function, and prints the result as required.

8. Simple Array Sum - https://www.hackerrank.com/challenges/simple-array-sum/problem?isFullScreen=true

solving method:

->The simpleArraySum function takes an array ar as input and uses the sum function to calculate the sum of the elements in the array.

->In the main part of the code, it reads the input, including the size of the array and the array elements.

->It calls the simpleArraySum function and assigns the result to the result variable.

->Finally, it writes the result to the output file.

9. Staircase - https://www.hackerrank.com/challenges/staircase/problem?isFullScreen=true

    solving method:

-> The staircase function takes an integer n as input and uses a loop to iterate from 0 to n - 1.

->For each step, it calculates the number of spaces and hash symbols needed in that step and prints them accordingly.

->The spaces are created using " " * (n - i - 1) to produce the appropriate number of spaces, and the hashes are created using "#" * (i + 1) to generate the hash symbols.

->It prints the combination of spaces and hash symbols for each step, creating the staircase pattern.

->In the main part of the code, it reads the input, which is the size of the staircase, and calls the staircase function to print the pattern.

10. Taum and B'day - https://www.hackerrank.com/challenges/taum-and-bday/problem?isFullScreen=true

     solving method:

 ->The taumBday function takes the number of black gifts b, the number of white gifts w, the cost of a black gift bc, the cost of a white gift wc, and the cost to convert one color gift to the other color z.

->It calculates the cost of buying black gifts separately (b * min(bc, wc + z)) and the cost of buying white gifts separately (w * min(wc, bc + z)).

->The function returns the sum of these two costs, which represents the minimum total cost.

->In the main part of the code, it reads the number of test cases t and iterates through each test case. For each test case, it reads the input parameters, calls the taumBday function to calculate the minimum cost, and writes the result to the output file.




































   


