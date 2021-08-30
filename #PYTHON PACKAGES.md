# PACKAGES IN PYTHON 

## PYTHON
 
Python is an interpreted high-level general-purpose programming language. Its design philosophy emphasizes code readability with its use of significant indentation. Its language constructs as well as its object-oriented approach aim to help programmers write clear, logical code for small and large-scale projects.


<img src="https://images.hdqwalls.com/download/python-logo-4k-i6-1920x1080.jpg" alt="COVID-19">



## PYTHON PACKAGES

This widespread usage is enabled, in part, by an extensive standard library that offers a range of facilities designed to enhance the functionality and portability of Python. This is complemented with a growing number of packages and projects available through the Python Package Index (PyPI), which not only provide extended capabilities of Python to more domain-specific use cases, but also increase the general usability of Python.


## FEW PYTHON PACKAGES

1.**Pip**: pip is the standard way of installing and managing packages in Python. Pip comes standard with every Python distribution, allowing you to accomplish installs, uninstalls, updates, etc from the command line. For example, to install a specific package with pip from PyPI, run:

pip install “SomePackage”
 

Or for a specific package version:

For example: pip install “SomePackage == 1.0”
 

pip allows for installation from multiple sources, and is not limited to installing packages maintained on the PyPI.

2.**Numpy**: We can do basic mathematical operations without any special Python packages. However, if you’re going to do any kind of complex math, the NumPy package will make your coding life much easier.

NumPy provides tools to help build multi-dimensional arrays and perform calculations on the data stored in them. You can solve algebraic formulas, perform common statistical operations, and much more.

For example: to create two 2×2 complex matrices and print the sum: 

import numpy as np

a = np.array([[1+2j, 2+1j], [3, 4]])
b = np.array([[5, 6+6j], [7, 8+4j]])
print(a+b)

3.**Pandas**: The pandas package introduces a novel data structure, the DataFrame, optimized for tabular, multidimensional, and heterogeneous data. Once your data has been converted to this format, the package provides intuitive and practical means to clean and manipulate it. 

Manipulations such as groupby, join, merge, concatenate data or filling, replacing and imputing null values can be executed in a single line. The developers of the package have the primary goal of producing the world’s most powerful data analysis and manipulation tool that exists in any language — a daunting task that they may actually achieve. 

For example: To create a DataFrame:

import pandas as pd

df_1 = pd.DataFrame({‘col1’: [1,2], ‘col2’: [3,4]})
 
 And to concatenate two dataframes together:

df_2 = pd.DataFrame({‘col3’: [5,6], ‘col4’: [7,8]})
df = pd.concat([df_1,df_2], axis = 1)

4.**Pendulum**: If you have at least a little Python programming experience, you probably know that you can use the datetime module to manage dates and times within an application.

While datetime is great for basic work along these lines, the Pendulum Python package makes it easier to do more complex coding involving dates and times. It’s more intuitive to work with, and it manages time zones automatically.

Best of all, Pendulum is designed to be a drop-in replacement for datetime. That means you can use it with code you’ve already written based on datetime. With only a few exceptions, Pendulum will work just as well, without the need to modify the code, while providing extra features not present in plain-old datetime.

For example: # import library
import pendulum
dt = pendulum.datetime(2020, 11, 27)
print(dt)

#local() creates datetime instance with local timezone
local = pendulum.local(2020, 11,27)
print(local)
print(local.timezone.name)


5.**Python Imaging Library**: If your Python application interacts with images in any way, the Python imaging library, also known as PIL or Pillow, is a Python must-have. It makes it easy to write code that opens, modifies, and saves images in a variety of formats.

If you’re doing more advanced work with images (like image recognition, in which case OpenCV would be a good package to consider), Pillow won’t cut it on its own. But for basic image importing, manipulation, and exporting, Pillow is your go-to solution.

For example: from PIL import Image


img = Image.open(r"test.png")
img.show()


6. **MoviePy**: MoviePy is to videos what Pillow is to images. It provides a range of functionality for common tasks associated with importing, modifying, and exporting video files. It also lets you do things like insert titles into videos or rotate videos 90 degrees (if for some reason you decide you want to do that).

Like Pillow, MoviePy is not intended as a tool for advanced data manipulation. If you’re writing a video editing app, you’ll probably also need to rely on OpenCV (which can work with videos as well as images) to provide the advanced functionality that MoviePy lacks. But for most standard tasks involving videos in Python code, MoviePy gets the job done quite well.

For example: # Import everything needed to edit video clips
from moviepy.editor import *

 #### loading video dsa gfg intro video
clip = VideoFileClip("dsa_geek.webm")

 #clipping of the video
 ##### getting video for only starting 10 seconds
clip = clip.subclip(0, 10)

 ##### rotatng video by 180 degree
clip = clip.rotate(180)

 ##### Reduce the audio volume (volume x 0.5)
clip = clip.volumex(0.5)

 ##### showing clip
clip.ipython_display(width = 280)

7.**tkinter**:  There are a variety of packages designed to help you do that (indeed, we could make a top ten list of just Python GUI packages). But I think most Python developers would agree that Tkinter is the most important — and most commonly used — framework for creating GUIs. It binds Python to the TK GUI toolkit, which works on virtually every modern operating system.

Unless you have a strong preference for a different GUI toolkit, Tkinter is probably the best place to start when creating a Python GUI.

For example: import tkinter as tk
r = tk.Tk()
r.title('Counting Seconds')
button = tk.Button(r, text='Stop', width=25, command=r.destroy)
button.pack()
r.mainloop()


8.**Pywin32**: For Windows Python programming in particular, Pywin32 is a must-have package. It provides access to many of the native Windows API functions, allowing you to do things like interact with the Windows registry, use the Windows clipboard, and much more.

Pywin32 won’t do you much good if you’re building a cross-platform Python app, but Windows developers might find that they like it so much that they use it instead of native Windows tooling.

 

 For Python module structured package: https://data-flair.training/blogs/python-packages/
 

