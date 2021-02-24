# Print N Lowest Numbers
## Prompt:
![Replr1](/images/n_lowest_numbers.png)

## Tools:
- [Repl.it](https://repl.it/) - "Replit is the best tool for quickly starting, sharing, and developing projects in any programming language, right from your browser."

## Solution:
The only challenging aspect of this challenge was mentually understanding how to work with arrays in C++. Where I am not very fluent with the language, and C++ doesn't have quite as many mechanisms to handle it's various built in classes as C#, or even Ruby, it took me a bit to mentally conceptualize how to store the temporary value. The code below iterates over the length of the array, grabs the Ith value from the array, then iterates over the array again and compares the Ith value to the Jth value. Which ever is smaller get's assigned to the Ith location in the array and swapped with the variable previously stored in the Ith (or Jth if smaller) location.

Final solution ([view on repl](https://repl.it/@zleavitt/Print-N-Lowest-Numbers)):
```cpp
#include <iostream>
#include <algorithm>

using namespace std;

void PrintNLowestNumbers(int arr[], unsigned int length, unsigned short nLowest)
{
  // print the n lowest numbers to stdout seperated by space character, do not de-dupe
  int i, j, min, temp;
  for (i = 0; i < length - 1; i++) {
    min = i;
    for (j = i + 1; j < length; j++)
      if (arr[j] < arr[min])
        min = j;
    temp = arr[i];
    arr[i] = arr[min];
    arr[min] = temp;
  }
  
  for (i = 0; i < nLowest; i++){
    cout << arr[i] << " ";
  }

}

int main()
{
	char input[0x100];
	int integerList[0x100];
	unsigned int length;
	unsigned short nLowest;
	std::cin >> nLowest;
	std::cin >> length;
	for (int i=0;i<length;i++)
		 std::cin >> integerList[i];
	PrintNLowestNumbers(integerList, length, nLowest);
}

// int main()
// {
// 	int integerList [8] = {5, 8, 0, 22, -2000, 8, 62, -26};
//   int length = 8;
//   int nLowest = 99;
// 	PrintNLowestNumbers(integerList, length, nLowest);
// }
```

Flag:
> There was no flag for this challenge, only the code listed above.