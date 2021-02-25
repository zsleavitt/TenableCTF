# The Only Tool You'll Ever Need
## Prompt:
![TheOnlyToolYoullEverNeed](/images/the_only_tool_youll_ever_need.png)

## Tools:
- [Ida 7.5 (Demo)](https://www.hex-rays.com/products/decompiler/)

## Solution:
The was by far one of the most interesting challenges that I worked on for the CTF. I ended up having to sign up for a demo of a tool called IDA however other than that the challenge itself wasn't that difficult. Here's how I solved the challenge:

1. Since the category of this challenge was Reverse Engineering I started by searching Google for "the only tool you'll ever need reverse engineering"
    1. ![TheOnlyToolYoullEverNeed1](/images/the_only_tool_youll_ever_need_1.png)
1. After reading through some of the introduction I skipped to the first result on [apriorit's top 10 list](https://www.apriorit.com/dev-blog/366-software-reverse-engineering-tools):
    1. ![TheOnlyToolYoullEverNeed2](/images/the_only_tool_youll_ever_need_2.png)
1. Next I signed up for a demo version of IDA 7.5, installed the program and launched it:
    1. ![TheOnlyToolYoullEverNeed3](/images/the_only_tool_youll_ever_need_3.png)
1. Following launch I clicked 'New', opened the 'a.out' attachment, and clicked 'Ok' at the following propmt:
    1. ![TheOnlyToolYoullEverNeed4](/images/the_only_tool_youll_ever_need_4.png)
1. And there was the flag, hidden in a comment embedded in the code of the program (sorry for the huge screenshot):
    1. ![TheOnlyToolYoullEverNeed5](/images/the_only_tool_youll_ever_need_5.png)

![TheOnlyToolYoullEverNeed6](/images/the_only_tool_youll_ever_need_6.png)

Flag:
> flag{str1ngs_FTW}