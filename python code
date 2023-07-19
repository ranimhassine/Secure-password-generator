import random
import string
import tkinter as tk
from tkinter import messagebox

def generate_password(length, complexity):
    characters = ""

    if "weak" in complexity.lower():
        characters += string.ascii_letters
    elif "medium" in complexity.lower():
        characters += string.ascii_letters + string.digits
    elif "strong" in complexity.lower():
        characters += string.ascii_letters + string.digits + string.punctuation

    password = ''.join(random.choice(characters) for _ in range(length))
    return password

def generate_button_clicked():
    try:
       length = int(length_entry.get())
       complexity = complexity_entry.get()
       
       password = generate_password(length, complexity)
       messagebox.showinfo("Generated Password", password)
    except ValueError:
       messagebox.showerror("Error", "Invalid password length")

root = tk.Tk()
root.title("Secure Password Generator")

length_label = tk.Label(root, text="Password Length:")
length_label.pack()

length_entry = tk.Entry(root)
length_entry.pack()

complexity_label = tk.Label(root, text="Complexity (weak/medium/strong):")
complexity_label.pack()

complexity_entry = tk.Entry(root)
complexity_entry.pack()

generate_button = tk.Button(root, text="Generate Password", command=generate_button_clicked)
generate_button.pack()

root.mainloop()
