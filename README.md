# command-line-arguments-to-count-word
## AIM:
To write a python program for getting the word count from the contents of a file using command line arguments.
## EQUIPEMENT'S REQUIRED: 
PC, Anaconda - Python 3.7
## ALGORITHM: 
1.Import sys module to use command line arguments

2.Use the open() by getting the file name with sys.argv[1] which means the first index of the given argument 

3.Iterate the content of the file using for loop

4.Split the contents into each line using split() function

5.Iterate the list of the line and increment the value of variable each time

6.Run the program by giving the file name on thr terminal

## PROGRAM:
```
#Developed by: Meetha Prabhu
#Reg No: 212222240065
import sys
count={}
with open(sys.argv[1],'r') as f:
    for line in f:
        for word in line.split():
            if word not in count:
                count[word]=1
            else:
                count[word]+=1
print(count)
f.close()
```
### OUTPUT:
File:

![image](https://github.com/Meetha22003992/command-line-arguments-to-count-word/assets/119401038/b531c5f8-4849-4fe4-9d23-48458ae4dd0a)

![image](https://github.com/Meetha22003992/command-line-arguments-to-count-word/assets/119401038/2c423646-68ba-40e4-a3d8-d20f2efc38bd)

## RESULT:
Thus the program is written to find the word count from the contents of a file using command line arguments.
