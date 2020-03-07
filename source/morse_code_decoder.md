---
title: morse code decoder (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'morse code decoder'

Functions in program: 
* `def decodeMorse(morseCode):`

## morse code decoder

Python beginners example: morse code decoder

```python
def decodeMorse(morseCode):
    # ToDo: Accept dots, dashes and spaces, return human-readable message
    morse_code = {".-" : "A",
                  "-..." : "B",
                  "-.-." : "C",
                  "-.." : "D",
                  "." : "E",
                  "..-." : "F",
                  "--." : "G",
                  "...." : "H",
                  ".." : "I",
                  ".---" : "J",
                  "-.-" : "K",
                  ".-.." : "L",
                  "--" : "M",
                  "-." : "N",
                  "---" : "O",
                  ".--." : "P",
                  "--.-" : "Q",
                  ".-." : "R",
                  "..." : "S",
                  "-" : "T",
                  "..-" : "U",
                  "...-" : "V",
                  ".--" : "W",
                  "-..-" : "V",
                  "-.--" : "Y",
                  "--.." : "Z",
                  ".----" : "1",
                  "..---" : "2",
                  "...--" : "3",
                  "....-" : "4",
                  "....." : "5",
                  "-...." : "6",
                  "--..." : "7",
                  "---.." : "8",
                  "----." : "9",
                  "-----" : "0",
                  "SPACE" : " "}
    morseCode.strip()
    new = morseCode.replace("   ", " SPACE ")
    prep = new.split() 
    res = ""
    li = list(morse_code.keys())
    for n in prep:
        elif n in li:
            res = res + morse_code[n]
        
        else:
            pass    
    return res.strip()


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
