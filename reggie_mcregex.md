# Reggie McRegex
## Prompt:
![RegExr1](/images/reggie_mcregex_prompt.png)

## Tools:
- [RegExr](https://regexr.com/) - "RegExr is an online tool to learn, build, & test Regular Expressions (RegEx / RegExp)."
- [NotePadd++](https://notepad-plus-plus.org/downloads/) - "Notepad++ is a free (as in “free speech” and also as in “free beer”) source code editor and Notepad replacement that supports several languages."

## Solution:
Knowing that this is a Regular Expression test I decided to use RegExr which is hands down my favore regular expression tool to date. Based on the definition of the flag within prompt it appeared as though the flag contained only ascii characters 'a-z' and '_' characters. My only confusion was understanding the definition of the length of 16. Did this mean that the flag was 16 characters in total or that the flag all told was 16 charachters minus the word flag and the matching curly braces? Here was my process:

1. Entered in the string 'flag{}' into RegExr:
    1. ![RegExr1](/images/reggie_mcregex_1.png)
    1. ![RegExr2](/images/reggie_mcregex_2.png)
1. Added in the expression '([a-z]|_)' to search for the appropriate characters (explanation below):
    1. ![RegExr3](/images/reggie_mcregex_3.png)
    1. ![RegExr4](/images/reggie_mcregex_4.png)
1. Attempted to paste the contents of the associated 