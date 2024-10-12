``` python
def sumOfPrimeFactors(n):
    # Initialize sum for prime factors
    prime_factor_sum = 0
    
    # Check for number of 2s that divide n
    while n % 2 == 0:
        prime_factor_sum += 2
        n //= 2
    
    # Now n must be odd, so we can skip even numbers
    for i in range(3, int(n**0.5) + 1, 2):
        # While i divides n, add i and divide n
        while n % i == 0:
            prime_factor_sum += i
            n //= i
    
    # This condition is to check if n is a prime number greater than 2
    if n > 2:
        prime_factor_sum += n
    
    return prime_factor_sum


n = 28
print(sumOfPrimeFactors(n))  # Output: 11
```




# Question 2
You are given a string 3gs representing server logs separated by a delilniter (e.g., ""), Identify the total count of logs containing the word "breach"
Note that the string may contain lowercase and uppercase letters, spaces, and digits (0-9).
Note also that the case of "breach" letters doesn't matter, so "BrEach", "Breach" or "brEACH" should be also counted.
For example, the answer for the string "breach brEach;; Breach" is 2, because the first and third logs contain the word "breach" at least once (the second log is empty because it's between two delimiters".
Functin description
Complete the findBreachCount function in the editor below. It has the following parameter(s):
Name
Type
Description
Answered
logs
STRING
Server logs separated by a delimiter, le the semicolon
Return
The function must return an INTEGER denoting the count of logs mentioning "breach".
Constraints
1 len(logs) $ 10^5
Input format for debugging
The first line contains a string, logs, denoting the server logs where each log is separated by a delimiter; i.e the semicolon
``` python
import sys

def findBreachCount(logs):
    # Step 1: Split the logs by semicolon into a list
    log_entries = logs.split(';')
    
    # Step 2: Initialize a counter for logs containing "breach"
    breach_count = 0
    
    # Step 3: Loop over each log and check if "breach" is present (case insensitive)
    for log in log_entries:
        if 'breach' in log.lower():  # convert to lowercase and check for "breach"
            breach_count += 1
    
    # Step 4: Return the total count
    return breach_count

def main():
    # Read the input string from stdin (trim the newline character at the end)
    logs = sys.stdin.readline().strip('\n')
    
    # Call the findBreachCount function
    result = findBreachCount(logs)
    
    # Output the result
    print(result)

if __name__ == "__main__":
    main()

```
