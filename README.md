# why-worry
Why Worry

https://www.youtube.com/watch?v=ngLEhVU1Ezk
----------------------------------------------------



import tkinter as tk
from tkinter import messagebox

def show_message(problem_exists, can_solve):
    why = "Then Why Worry?"
    if not problem_exists or can_solve:
        messagebox.showinfo("Message", why)
    else:
        messagebox.showinfo("Message", why)
import tkinter as tk
from tkinter import messagebox

def show_message(problem_exists, can_solve):
    why = "Then Why Worry?"
    if not problem_exists or can_solve:
        messagebox.showinfo("Message", why)
    else:
        messagebox.showinfo("Message", why)

def ask_second_question():
    response = messagebox.askyesno("Question", "Can You Do Something About It?")
    show_message(True, response)

def ask_first_question():
    response = messagebox.askyesno("Question", "Do You Have a Problem In Life?")
    if response:
        ask_second_question()
    else:
        show_message(False, None)

def main():
    root = tk.Tk()
    root.title("Why Worry Project")
    
    tk.Button(root, text="Start", command=ask_first_question).pack(pady=20)
    
    root.mainloop()

if __name__ == "__main__":
    main()

if __name__ == "__main__":
    main()
