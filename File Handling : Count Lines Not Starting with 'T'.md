# File Handling in Python: Count Lines Not Starting with 'T'

## 🎯 Aim
To write a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'`.

## 🧠 Algorithm
1. Open the file `story.txt` in **read mode**.
2. Initialize a counter `count` to zero.
3. Iterate through each line of the file:
   - Check if the first character of the line is **not** `'T'`.
   - If the line does not start with `'T'`, increment the `count` by 1.
4. After processing all lines, print the `count` value, which represents the number of lines that do not start with `'T'`.

## 🧾 Program
```
try:
    with open('story.txt', 'r') as file:
        count = 0  
        for line in file:
            if not line.lstrip().startswith('T'):
                count += 1
    print(f"Number of lines not starting with 'T': {count}")

except FileNotFoundError:
    print("The file 'story.txt' was not found.")
```
## Output
<img width="1258" height="298" alt="image" src="https://github.com/user-attachments/assets/9d79c59f-b14f-4112-9d15-be66476b7284" />

## Result
the code is executed
