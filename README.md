The .py file contains two classes that create random passwords based on the set parameters of the object. I used the os, random, and string modules. 

for each class below I listed the functions to control the parameters of the object.

the first class, memorablePass, makes them out of a set number of words and numbers that are connected by a hyphen. this can be set to include both capital and lowercase or just capital/just lowercase.

def setNumWords(self, x: int):
        self.numwords=x

def setMultiCases(self, cases: bool):
        self.multicases=cases

def setDefaultCase(self, default: bool):
        self.defaultcase=default

        
the second class, randomPass, uses a set length of random letters and numbers, and also puntuation if the variable is set to true. You can also use the setNotIncluded function to give a string of characters you don't want in the passwords.

def setlength(self, x: int):
        self.length=x

def setPunc(self, punc: bool):
        self.punctuation=punc

def setNotIncluded(self, notInc: str):
        self.notIncluded=notInc


for both classes there is a generate(self, num: int) function that takes the variable "num" as the number of passwords it should make and save to the txt file. 

I made this program on an IUI Library computer which didn't have conda installed so I wasnt able to create a virtual environment to save the file in, so I just had all the files as being in my Documents directory.
If that is unable to save the passwords I also have commented out print statements in the generate functions that could show what is being generated.
