# Digital-Time
✅Created a World Digital Time GUI using Python! It continuously shows the time as the day goes by. Feel free to experience it. Thank you!
![image](https://github.com/FortuneAdeleye/Digital-Time/assets/142922953/627f82b5-d8c5-49a0-abae-80a2ef54fd66)


# Import Libraries:
- from tkinter import *
- from tkinter.ttk import *
- from time import strftime
- I used these imports because they bring in the necessary modules for creating the GUI (tkinter and tkinter.ttk) and for getting the current time (strftime from the time module).

# Initialize the Root Window:
- root = Tk()
- root.title("Clock")
- Creates the main window of the application and sets the window title to "Clock".

# Define the Time Function:
- def time():
- string = strftime("%I:%M:%S %p")
- label.config(text=string)
- label.after(1000, time)
- I used this function to get the current time in the format HH:MM:SS AM/PM using strftime.
- Updates the text of the label with the current time.
- Uses label.after(1000, time) to call the time function again after 1000 milliseconds (1 second) to continuously update the time.

# Create and Pack the Label:
- label = Label(root, font=("ds-digital", 80), background="black", foreground="cyan")
- label.pack(anchor="center")
- I used this to create a label widget with a digital font style, a large font size, a black background, and cyan-colored text.
- Packs (adds) the label to the window, centering it in the main window.

# Call the Time Function and Start the Main Loop:
- time()
- mainloop()
- I put this at the end of my code so that it calls the time function to start the initial time update.
- Starts the mainloop, which keeps the application running and responsive.
- This code sets up a simple digital clock that updates every second and displays the time in a large, easily readable format.






