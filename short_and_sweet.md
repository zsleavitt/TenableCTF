# Short and Sweet
## Prompt:
![Replr1](/images/short_and_sweet_prompt.png)

## Tools:
- [Repl.it](https://repl.it/) - "Replit is the best tool for quickly starting, sharing, and developing projects in any programming language, right from your browser."

## Solution:
The solution to this problem was relative easy however, this was probably by design where the flag was only worth 25 points. The key to this solution is understanding the modulus operator, which attmepts to divide a number by another number and returns the remainder from the operation. Therefore this code is as simple testing each number to check if it is divisible (modulus) by 2. 

Final solution ([view on repl](https://repl.it/@zleavitt/Short-and-Sweet)):
```python
def AreNumbersEven(numbers):
  isEvenList = []
  for number in numbers:
    if (number % 2) == 0:
      isEvenList.append(True)
    if (number % 2) != 0:
      isEvenList.append(False)
  
  return isEvenList

# Read space delimited integers from stdin and 
# pass a list of them to AreNumbersEven()
numbers = raw_input()
integer_list = [int(i) for i in numbers.split(' ')]
even_odd_boolean_list = AreNumbersEven(integer_list)
print even_odd_boolean_list 
```

Flag:
> There was no flag for this challenge, only the code listed above.

### Notes:
This solution isn't the optimal solution where it performs 2 comparisons to see if the number is divisible by zero. 