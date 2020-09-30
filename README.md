# flight-gui
Analyse flights 
from tkinter import *
import os
import sys

root = Tk()

root.geometry("300x200")
root.minsize(300,200)
root.maxsize(300,200)
root.title("D-Labz Aerospace Flight Deta Analwzer ")

def Dark():
    os.system('cmd /k "dark.py"')
    
def Light():
    os.system('cmd /k "light.py"')
    

l1=Label(root,text="").pack()
l=Label(root,text="Choose your preferred theme", font="Helvetica 15 bold").pack()

b1=Button(text="LIGHT THEME", command=Light, font="Helvetica 10 bold").pack(pady=10)
b2=Button(text="DARK THEME", command=Dark, font="Helvetica 10 bold", fg="white",bg="#35363A").pack()
 
root.mainloop()
