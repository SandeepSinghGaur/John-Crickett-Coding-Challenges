# JSON Parser Challenge

## Introduction
This challenge is to build your own JSON parser. Building a JSON parser is an excellent way to learn about parsing techniques, which are useful for everything from parsing simple data formats to building fully featured compilers for programming languages.

Parsing is often broken up into two stages: lexical analysis and syntactic analysis. Lexical analysis divides a sequence of characters into meaningful chunks called tokens. Syntactic analysis (parsing) analyzes the list of tokens to match it to a formal grammar.

For more about building lexers, parsers, and compilers, refer to "Compilers: Principles, Techniques, and Tools" (widely known as the "Dragon Book").

## The Challenge - Building a JSON Parser

JSON (JavaScript Object Notation) is a lightweight data-interchange format, widely used for transmitting data over the Internet. It is formally defined by the IETF here: [IETF JSON](https://tools.ietf.org/html/std90). You can also refer to a simpler graphical representation here: [JSON.org](https://www.json.org/json-en.html).

### Step Zero
Set up your environment ready to begin developing and testing your solution. Choose your IDE/editor and programming language of choice. Download simple test data for the JSON parser from the provided link.

### Step 1
In this step, your goal is to parse a valid simple JSON object, specifically: `{}` and an invalid JSON file, and correctly report which is which. Build a very simple lexer and parser for this step.

Your program should:
- Report to the standard output stream a suitable message.
- Exit with code `0` for valid and `1` for invalid.

You can test your code against the files in the folder `tests/step1`. Consider automating the tests so you can run them repeatedly as you progress through the challenge.

### Step 2
Extend the parser to parse a simple JSON object containing string keys and string values, i.e.:

```json
{"key": "value"}
```
### Step 3

```
{
  "key1": true,
  "key2": false,
  "key3": null,
  "key4": "value",
  "key5": 101
}
```
### Step 4

```
{
  "key": "value",
  "key-n": 101,
  "key-o": {},
  "key-l": []
}
```