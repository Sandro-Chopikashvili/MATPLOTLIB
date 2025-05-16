# 📊 Matplotlib Basic Plot Example

This repository contains a simple Python script demonstrating how to create basic line plots using Matplotlib and NumPy. 🐍📈

## 📝 Description

The script `SinCos.ipynb` generates and plots the sine and cosine functions over 100 evenly spaced points between 0 and 10.

It showcases how to:

- Generate data points with NumPy (`linspace`, `sin`, `cos`) ➡️
- Create line plots with Matplotlib 🎨
- Customize plot appearance (colors, line styles, labels, title) ✏️
- Add grid lines and legends 📋
- Save plots as image files 💾

## 🚀 Usage

1. Make sure you have Python installed (Python 3.6+ recommended). 🐍  
2. Install the required libraries if you don’t have them:

 ```bash
pip install matplotlib numpy
 ```


## 📝 Code 
```py
import matplotlib.pyplot as plt
import numpy as np

x = np.linspace(0, 10, 100)
y1 = np.sin(x)
y2 = np.cos(x)

plt.figure(figsize=(10, 6))

plt.plot(x, y1, label='sin(x)', color='blue', linestyle='-')
plt.plot(x, y2, label='cos(x)', color='red', linestyle='--')

plt.title('Sine and Cosine Functions')
plt.xlabel('x values')
plt.ylabel('Function values')

plt.legend()
plt.savefig("sine_cosine_plot.png")  
```

![Sine and Cosine Functions](Source/sine_cosine_plot.png)
