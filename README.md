# Sum-of-sum-of-integers
Raj wrote all the integers from 1 to n on a paper (inclusive). Then he replaced each integer with the sum of its digits. What will be the sum of number written now on the page? You're given the integer n.   Input An integer n. ( 1 &lt;= n &lt;= 1e4). Output Print the sum as described in the question.

def digit_sum(num):
    return sum(map(int, str(num)))

def sum_of_digit_sums(n):
    result = 0
    for i in range(1, n + 1):
        result += digit_sum(i)
    return result
n = int(input())
result = sum_of_digit_sums(n)
print(result)
