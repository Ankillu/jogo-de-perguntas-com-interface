from tkinter import Tk
from tkinter import *
import tkinter as tk
from tkinter import messagebox

root1 = tk.Tk()
root1.geometry("512x512")
root1.wm_title("5 elevado a 5")
labeldapergunta1 = tk.Label(root1, text="Quanto é 5 elevado a 5")
entradaderesposta1 = tk.Entry(root1)
botãodeconfirmarresposta1 = tk.Button(root1, text="clique aqui pra confirmar")
labeldapergunta1.pack()
entradaderesposta1.pack()


def confirmarresposta1(pergunta1):
    if pergunta1 == "3125":
        root2 = tk.Toplevel(root1)
        entradaderesposta2 = tk.Entry(root2)
        root2.geometry("512x512")
        root2.wm_title("4 elevado a 3")
        labeldapergunta2 = tk.Label(root2, text="Quando e 4 elevado a 3")
        labeldapergunta2.pack()
        entradaderesposta2.pack()
        entradaderesposta2.focus_set()
        botãodeconfirmarresposta2 = tk.Button(
            root2, text="clique aqui pra confirmar", command=lambda: confirmarresposta2(entradaderesposta2.get()))
        botãodeconfirmarresposta2.pack()
        root2.mainloop()
    else:
        messagebox.showerror("Erro", "Você errou!")


def confirmarresposta2(answer):
    if answer == "64":
        messagebox.showinfo("Você acertou tudo")
    else:
        messagebox.showerror("Você errou!")


botãodeconfirmarresposta1.config(command=lambda: confirmarresposta1(entradaderesposta1.get()))
botãodeconfirmarresposta1.pack()
root1.mainloop()
