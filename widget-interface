from tkinter import *
import tkinter.messagebox as box

# Use app name throughout
appname='Thorganizer'

window = Tk()
window.title(appname)
label = Label(window, text='What is running through your mind?')
label.pack(padx=200, pady=50)

frame = Frame(window)
entry = Entry(frame, width=200)

listbox = Listbox(frame)
listbox.insert(1, 'ANT')
listbox.insert(2, 'Fact')
listbox.insert(3, 'Idea')
listbox.insert(4, 'Info')
listbox.insert(5, 'Realisation')


def dialog():
        box.showinfo('Thought: ' + entry.get() + 'Class: ' + listbox.get( listbox.curselection() ))

btn = Button(frame, text='Add content', command=dialog)

img = PhotoImage(file = 'THORG.gif')

can = Canvas(window, width=100, height = 100)
can.create_image((50, 50), image= img)

entry.pack()
frame.pack(padx=20, pady=20)
listbox.pack(padx=5)
btn.pack(padx=5, pady=5)
can.pack(padx=2, pady=2)

box.pack(padx=2, pady=2)


window.mainloop()
