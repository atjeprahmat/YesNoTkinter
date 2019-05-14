# YesNoTkinter

Mencoba desain sederhana python menggunakan Tkinter, tidak usah repot repot menggunakan IDE yang anda sukai cukup menggunakan IDLE PYTHON bawaan setelah anda install python,
lalu buat dokumen baru sisipkan sintaks berikut, lalu run module, cukup mudah silakan di coba..

    import tkinter as tk
    from tkinter import messagebox

    root= tk.Tk()

    canvas1 = tk.Canvas(root, width = 800, height = 350)
    canvas1.pack()

    def ExitApplication():
        MsgBox = tk.messagebox.askquestion('Exit Application','Are You Sure Want to Exit?', icon='warning')
        if MsgBox == 'yes':
            root.destroy()
    else:
        tk.messagebox.showinfo('Return','You Will Now Return to the Application Screen')

    button1 = tk.Button (root, text='Exit Application', command=ExitApplication)
    canvas1.create_window(97, 270, window=button1)

