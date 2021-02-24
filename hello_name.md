# Hello Name
## Prompt:
![Replr1](/images/hello_name_prompt.png)

## Tools:
- [Repl.it](https://repl.it/) - "Replit is the best tool for quickly starting, sharing, and developing projects in any programming language, right from your browser."

## Solution:
This was definitely the easiest of the programming problems, however due to my infamiliariy with C++, and the fact that I haven't worked with it in years, it took me longer than I expected. Basically the solution to this challenge was just to regurgitate the users name after they entered it into the input. Since the challenge didn't specify any validation, I did just that.

Final solution([view on repl](https://repl.it/@zleavitt/Hello-dollarname-1)):
```cpp
#include <stdio.h>
#include <iostream>

int main()
{
   std::string name = ""; 
   std::cin >> name;
   std::cout << "Hello " << name;
  return 0;
}
```

Flag:
> There was no flag for this challenge, only the code listed above.