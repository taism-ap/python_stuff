# Random Python Specifics


## Offline IDE (IDLE, Anaconda, etc)

If you create a basic program in python, it is easy to run either direction from the IDE or using the python command, i.e. "python3 program.py".

```python
x = "Hello World!"
print(x)
```
```
Hello World!
```

But what if instead I want my code inside a function

```python
def main():
  x = "Hello World!"
  print(x)
```

Now, if I try to run this program ("python3 program.py") 
```
```

nothing will happen, since I am not calling the function. You can fix this one of two ways. The first is to just call the function at the end of the program file:

```python
def main():
  x = "Hello World!"
  print(x)
main()
```

The second is to include something like this at the end of your program:

```python
def main():
  x = "Hello World!"
  print(x)

if __name__ == "__main__":
  main()
```

Why, you might ask, would you do this, if just adding "main()" at the end is easier? Good question.
