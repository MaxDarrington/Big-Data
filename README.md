# Big-Data
This is a python code designed to read an Excel spredshit composed of historical stock prices for the company, Amazon, 
and with the help of packages such as Pandas and Mathplot I will draw some analysis from this data.

Firstly, I imported Pandas as pd. I used the read_excel function to bring the data into a dataframe. 
With the following code I color coded the daily returns, red being negative and green being positive. 

def color_negative_red(value):
  if value < 0:
    color = 'red'
  elif value > 0:
    color = 'green'
  else:
    color = 'black'
  return 'color: %s' % color
  
  I used the .pct_change() to do the calculation. 
  
  Uppon adding the Daily Returns column into the dataframe, I plotted a historgram using the matplotlib package.
  This showed the dispursment of daily movements of the stock Amazon. 
