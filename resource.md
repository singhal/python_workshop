### Resource
I wrote up this resource list for you all: https://github.com/singhal/python_workshop/blob/master/Python.Md


### Dictionaries



### Function Practice

- Write a function that takes two numbers as arguments and returns the larger of the two. If the two numbers are equal, you can decide what to do.
- Write a function that takes a letter and returns `True` if it is a vowel.
	- Hint: Python can check if something is in a list, for example:
		```
		if my_number in [0, 1, 2, 3]:
			return True
		``` 
	- Hint: `True` is built-in Python constant, and you can treat it like anything else
- Define a function `mean(list)` that takes in a list of numbers and returns the mean of the numbers.
- Write a function that takes a list of integers and prints a histogram to the screen.

	- Hint: It should like like this. If given `values = [5, 6, 2]`, you would print:

		```
		*****
		******
		**
		```
	- Hint: See what happens when you do: `'a' * 5` in Python.
- Define a function `isPrime(number)` that takes in a number as argument and return `True` if the number is a prime number.

	- Hint: might be useful to know that this `%` is a special mathematical operation in Python. Play around with it in Python to see what it does.
- Define a function `get_counts(list)` that takes a list of words and returns a dictionary of the lengths of the words. For example, if given, `animals = ['cat', 'ant', 'zebra', 'elephant']`, you would return `counts = {'cat': 3, 'ant': 3, 'zebra': 5, 'elephant': 8}`.
- In cryptography, a Caesar cipher is a very simple encryption techniques in which each letter in the plain text is replaced by a letter some fixed number of positions down the alphabet. For example, with a shift of 3, A would be replaced by D, B would become E, and so on. The method is named after Julius Caesar, who used it to communicate with his generals. ROT-13 ("rotate by 13 places") is a widely used example of a Caesar cipher where the shift is 13. In Python, the key for ROT-13 may be represented by means of the following dictionary:

	```
	key = {	'a':'n', 'b':'o', 'c':'p', 'd':'q', 'e':'r', 'f':'s', 'g':'t', 'h':'u', 
       		'i':'v', 'j':'w', 'k':'x', 'l':'y', 'm':'z', 'n':'a', 'o':'b', 'p':'c', 
       		'q':'d', 'r':'e', 's':'f', 't':'g', 'u':'h', 'v':'i', 'w':'j', 'x':'k',
       		'y':'l', 'z':'m', 'A':'N', 'B':'O', 'C':'P', 'D':'Q', 'E':'R', 'F':'S', 
       		'G':'T', 'H':'U', 'I':'V', 'J':'W', 'K':'X', 'L':'Y', 'M':'Z', 'N':'A', 
       		'O':'B', 'P':'C', 'Q':'D', 'R':'E', 'S':'F', 'T':'G', 'U':'H', 'V':'I', 
       		'W':'J', 'X':'K', 'Y':'L', 'Z':'M'}
     ```
  Your task in this exercise is to implement an encoder/decoder of ROT-13. Once you're done, you will be able to read the following secret message: `Pnrfne pvcure? V zhpu cersre Pnrfne fnynq!`
	- Copied from _http://www.ling.gu.se/~lager/python_exercises.html_


### Data Analysis!
- We are going to analyze the data that are here: https://github.com/singhal/python_workshop
	- Right-click on the file named `cell_phone_subscriptions_100.csv` and save to your Desktop.
- First, we have to figure out how to read the data in.
	- Hint: the function `open()` will be useful!
- How many countries are in this data set?
	- Hint: you will likely need a dictionary!
	- Hint: you will need the function `split`
- What is the span of years represented in this data set?
	- Hint: when Python reads in text, it doesn't know a piece of text is a number unless you tell it to treat that text like a numerical variable.
- What is the maximum number of cell phone subscriptions across all years?
- What is the median number of cell phone subscriptions in 2011?
	- Hint: You might want to look into using `numpy`.
- Plot a histogram of cell phone subscriptions in 2005.
	- Hint: You might want to look into using `matplotlib.pyplot`.
- Plot a line plot of cell phone subscriptions in America and China through time.
- What is the average rate of increase in cell phone subscriptions across countries from 2010 to 2011?
- BRIC refers to Brazil, Russia, India, and China, or four countries that are considered to be emerging markets. What is the average rate of increase in cell phone subscriptions across only these four countries from 2010 to 2011?
- What country had 50% of its users with cell phone subscriptions first?
- CHALLENGE: Plot changes in cell phone subscriptions in Brazil through time. Is this best fit by a linear or exponential model? Fit the better model to the data.
