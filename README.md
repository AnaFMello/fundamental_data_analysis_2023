# fundamental_data_analysis_2023
# Ana Mello


Task 1 - The Collatz conjecture

The collatz_sequence Function takes a positive iteger n as starting point and calculates the collatz sequence for that number. 
def collatz_sequence(n):

It's process start with the number n and the calculation repets till gets the number 1.
    sequence = [n]

For even numbers, the number is divided by 2 and add the result to a list named sequence. 
    while n != 1:
        if n % 2 == 0:
            n = n // 2

If it's an odd number, it's multiplied by 3 and add 1, so the result returns as n
        else:
            n = 3 * n + 1
        sequence.append(n)
    return sequence

This process happens on a loop till n become 1. 

The verify_collatz_conjecture Function verifies the collatz conjecture for the limit positive integers, which in this case is definied 10,000.
def verify_collatz_conjecture(limit):
...
verify_collatz_conjecture(10000)

The for loop go through the positive integers from 1 to the limit.     
for i in range(1, limit + 1):

For eache intefer i, the function calls the collatz_sequence to calculate the collatz sequence for that integer. 
        sequence = collatz_sequence(i)

If the last number in the sequence is not 1, it meand the conjucture is false for that number and will print a message. 
        if sequence[-1] != 1:
            print(f"Collatz conjecture is not true for {i}")

If the last number is 1, it means the conjucture is true and will print a message. 
    print("Verification complete. The conjecture is true for the first 10,000 positive integers.")


## Search source
https://www.quantamagazine.org/why-mathematicians-still-cant-solve-the-collatz-conjecture-20200922/

https://www2.ifsc.usp.br/portal-ifsc/a-conjectura-de-collatz/
Explains the collatz conjecture

https://www.youtube.com/watch?v=1RL1ehEdLz4
Explains how to calculate

