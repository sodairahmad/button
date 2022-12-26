# button
how to create a button

from tkinter import *
window= Tk()
photo = PhotoImage(file='image.png')
count=0
def add():
    global count
    if count<3:
        x = int(input("enter ist number "))
        y = int(input("enter ist number "))
        print(f" The Sum of {x}  and {y}  is {x + y}")
        count += 1


button=Button(window, text='click me',command=add,font='Arial,30,bold',fg='#00FF00',bg='black'
              ,activebackground='black',activeforeground='#00FF00',state=ACTIVE,
              compound='top',image=photo)
button.pack()



window.mainloop()
