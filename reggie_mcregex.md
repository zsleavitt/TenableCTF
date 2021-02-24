# Reggie McRegex
## Prompt:
Find the flag in the attached file containing a haystack. Not including the quotes, the flag will be in the format of "flag{here_is_a_flag}". The text between the curly braces can consist of lowercase characters and underscores and be a maximum length of 16. You'll know it when you see it.

## Tools:
- [RegExr](https://regexr.com/) - "RegExr is an online tool to learn, build, & test Regular Expressions (RegEx / RegExp)."
- [NotePadd++](https://notepad-plus-plus.org/downloads/) - "Notepad++ is a free (as in “free speech” and also as in “free beer”) source code editor and Notepad replacement that supports several languages."

## Solution:
Knowing that this is a Regular Expression test I decided to use RegExr which is hands down my favore regular expression tool to date. Based on the definition of the flag within prompt it appeared as though the flag contained only ascii characters 'a-z' and '_' characters. My only confusion was understanding the definition of the length of 16. Did this mean that the flag was 16 characters in total or that the flag all told was 16 charachters minus the word flag and the matching curly braces? Here was my process:

1. Enter in the string 'flag{}' into RegExr:
    1. ![RegExr1](/images/reggie_mcregex_1.png)
    1. ![RegExr2](/images/reggie_mcregex_2.png)