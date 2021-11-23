# Python Regular Expressions Tutorial

-Regular Expressions, often shortened as regex, are a sequence of characters used to check whether a pattern exists in a given text (string) or not.

```python 
import re  # re is a library provide usefull function for regex as : compile(), search(), findall(), sub() for search and replace, split()

pattern = r"Cookie"   # r means raw text
sequence = "Cookie"
if re.match(pattern, sequence):   # match return True or False .. it try to fing if that text containing the pattern
    print("Match!")
else: print("Not a match!")
```

- [abc] - Matches a or b or c.

- [a-zA-Z0-9] - Matches any letter from (a to z) or (A to Z) or (0 to 9).

- \w - Lowercase 'w'.  Matches any single letter, digit, or underscore.

- \W - Uppercase 'W'. Matches any character not part of \w (lowercase w).

- \s - Lowercase 's'. Matches a single whitespace character like: space, newline, tab, return.

- \S - Uppercase 'S'. Matches any character not part of \s (lowercase s).

- \d - Lowercase d. Matches decimal digit 0-9.

- \D - Uppercase d. Matches any character that is not a decimal digit.

- \t - Lowercase t. Matches tab.

- \n - Lowercase n. Matches newline.

- \r - Lowercase r. Matches return.

- \A - Uppercase a. Matches only at the start of the string. Works across multiple lines as well.

- \Z - Uppercase z. Matches only at the end of the string.

- {x} - Repeat exactly x number of times.

- {x,} - Repeat at least x times or more.

- {x, y} - Repeat at least x times but no more than y times.

# shutil

```python 
import shutil
shutil.copyfile(path_to_copy_from , path_to_copy_to ) # copy file 
shutil.copymode(path_to_copy_from , path_to_copy_to ) # copy metadata 
```




https://www.datacamp.com/community/tutorials/python-regular-expression-tutorial

https://pymotw.com/3/shutil/