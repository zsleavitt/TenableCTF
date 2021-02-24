# Reggie McRegex
## Prompt:
![RegExr1](/images/reggie_mcregex_prompt.png)

## Tools:
- [RegExr](https://regexr.com/) - "RegExr is an online tool to learn, build, & test Regular Expressions (RegEx / RegExp)."

## Solution:
Knowing that this is a Regular Expression test I decided to use RegExr which is hands down my favorite regular expression tool to date. Based on the definition of the flag within the prompt it appeared as though the flag contained only the ascii characters 'a-z' and '_' characters. My only confusion was understanding the definition of the length being set at 16. Did this mean that the flag was 16 characters in total or that the flag was 16 characters all told minus the word flag and the matching curly braces? Here was my process:

1. Entered in the string 'flag{}' into RegExr:
    1. ![RegExr1](/images/reggie_mcregex_1.png)
    1. ![RegExr2](/images/reggie_mcregex_2.png)
1. Added in the expression '([a-z]|_)' to search for the appropriate characters (explanation below):
    1. ![RegExr3](/images/reggie_mcregex_3.png)
    1. ![RegExr4](/images/reggie_mcregex_4.png)
1. Added the number of characters to take into account when searching for the preceeding tokens (guessed 16):
    1. ![RegExr5](/images/reggie_mcregex_5.png)
    1. ![RegExr6](/images/reggie_mcregex_6.png)
1. Attempted to paste the contents of the associated haystack.txt into the RegExr 'Tests' section:
    1. ![RegExr6](/images/reggie_mcregex_7.png)

Final solution:
> flag{([a-z]|_){16}}

Flag:
> flag{thy_flag_is_this}