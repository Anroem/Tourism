# Tourism
I want to link guide and client in my project Tourism

import tkinter as tk
from tkinter import Button

def onclick(args):
    if args ==1:
        name = input("Enter all your name: \n")
        a = len(name)
        age = input("enter your age: ")
        password = input("enter your mot de password: ")
        retype = input("retype your password: " )
        email = input("enter your email: ")
        username = name + age
        print(username)

    if args ==2:
        name = input("Enter all your name: \n")
        a = len(name)
        age = input("enter your age: ")
        password = input("enter your mot de password: ")
        retype = input("retype your password: ")
        email = input("enter your email: ")

        username = name + age
        print(username)


root = tk.Tk()
root.title("Tourism")
btn1= tk.Button(root, text="Client", command=lambda :onclick(1))
btn2= tk.Button(root, text="Guide", command=lambda : onclick(2))

btn1.pack()
btn2.pack()
root.mainloop()
