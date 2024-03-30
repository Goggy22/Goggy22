python
Copy code
import tkinter as tk
from tkinter import messagebox

class DataCollectionApp:
    def __init__(self, master):
        self.master = master
        master.title("Data Collection App")

        self.label = tk.Label(master, text="Enter Data:")
        self.label.pack()

        self.entry = tk.Entry(master)
        self.entry.pack()

        self.submit_button = tk.Button(master, text="Submit", command=self.submit_data)
        self.submit_button.pack()

    def submit_data(self):
        data = self.entry.get()
        # Here you can do whatever you want with the collected data, like saving to a file or a database
        messagebox.showinfo("Data Collected", f"Data '{data}' collected successfully!")

def main():
    root = tk.Tk()
    app = DataCollectionApp(root)
    root.mainloop()

if __name__ == "__main__":
    main()
<!---
Goggy22/Goggy22 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
