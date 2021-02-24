# Esoteric
## Prompt:
![Esoteric](/images/esoteric_prompt.png)

## Tools:
- [Trusty Rusty Google](https://www.google.com)
- [Brainf*** Interpterer and Tape Visualizer](https://fatiherikli.github.io/brainfuck-visualizer/#LS1bLS0tLS0+KzxdPi4rKysrKysuLS0tLS0tLS0tLS0uKysrKysrLlstLS0tLT4rPF0+Li0tLS0uLS0tLisrK1stPisrKzxdPisuLS0tLS0tLS4rKysrKysrKysrLisrKysrKysrKysuKytbLT4rKys8XT4uKysrLlstLS0+KzxdPi0tLS0uKysrWy0+KysrPF0+KysuKysrKysrKysuKysrKysuLS0tLS0tLS0uLVstLS0+KzxdPi0tLitbLT4rKys8XT4rLisrKysrKysrLj4tLVstLT4rKys8XT4uCg==) - It appears as though this website processes... brainf***. 

## Solution:
I had virtually no knowledge about... this before going into the challenge. All I could really tell about it was that it looked to be like some kind of morse code. By pasting the string from the flag into Google, the first result was the "Brainf*** Language - Online Decorder, Translator, Interpreter" (sorry kids). This is how I arrived at the solution:

1. Browsed to Google and punched in the prompt's text:
    1. ![Esoteric1](/images/esoteric_1.png)
1. The text automatically populated in the interpreter, I just clicked run:
    1. ![Esoteric2](/images/esoteric_2.png)
1. Instead of waiting for the interpreter to parse the conents of the message I turned the 'Delay' slider all the way town, turned on the 'Optimize?' option and checked the '!' option (whatever that does). Thus we arrive at our result, sorry again kids:
    1. ![Esoteric3](/images/esoteric_3.png)

Flag:
> flag{wtf_is_brainfuck}