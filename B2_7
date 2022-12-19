import time
import urllib.request
import tkinter as tk
from tkinter import messagebox

root = tk.Tk()
root.wm_attributes("-topmost", True)
root.withdraw()


def check_internet_connection():
    try:
        # Try to open a website using urllib
        urllib.request.urlopen('http://www.google.com')
        return True
    except urllib.error.URLError:
        return False


while True:
    if check_internet_connection():
        pass
        # Do something here if the internet connection is available
    else:
        messagebox.showerror("Error", "Internet is not working!")
        # Do something here if the internet connection is lost

    # Wait for 10 seconds before checking again
    time.sleep(10)
