from tkinter import *

wn = Tk()

wn.geometry("500x500")

wn.title("To-Do List")

title_lbl = Label(text = "To-Do List", font = ("Georgia",85,"bold"))
title_lbl.pack()

list_frame = Frame(wn)
list_frame.pack(pady = 20)

to_do_list = Listbox(list_frame,
    font = "Cambria",
    width = 50,
    height = 5,
    bg = "SystemButtonFace",
    bd = 0,                  
    highlightthickness = 0,
    activestyle = "none")

to_do_list.pack()

to_do = ["Do math homework", "Exercise", "Read english assignment"]

for item in to_do:
    to_do_list.insert(END, item)

item_entry = Entry(wn, font = ("Georgia", 35))
item_entry.pack(pady = 20)

button_frame = Frame(wn)
button_frame.pack(pady = 20)

def add_item():
    to_do_list.insert(END, item_entry.get())
    item_entry.delete(0, END)

def delete_item():
    to_do_list.delete(ANCHOR)

def clear_item():
    to_do_list.delete(0,END)

add_button = Button(button_frame, text = "Add Item", font = ("Cambria", 12), width = 12, command = add_item)
delete_button = Button(button_frame, text = "Delete Item", font = ("Cambria", 12), width = 12, command = delete_item)
clear_button = Button(button_frame, text = "Clear", font = ("Cambria", 12), width = 12, command = clear_item)

add_button.grid(row = 0, column = 0)
delete_button.grid(row = 0, column = 1, padx = 10)
clear_button.grid(row = 0, column = 2)

wn.mainloop()
