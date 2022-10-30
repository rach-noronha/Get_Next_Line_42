<h1 align="center">
	Get_Next_Line_42 🚀
</h1>

<p align="center">
	<b><i>Let's deal with memory allocation!</i></b>
</p>

<p align="center">
  <img src="https://c.tenor.com/8XHjYF26qQQAAAAC/girl-pixel.gif" display="inline-block" width="40%" height="30%">
</p>

## 💡About

>Summary:
This project is about programming a function that returns a line
read from a file descriptor.

_Note: Files suffixed with *_bonus* are exact copies of corresponding files, except 'get_next_line_bonus.c"._

**Functions in `get_next_line.c`**

* `ft_read`	- copy read line from buffer to the static variable as much as needed until it finds an \n.
* `ft_return_line`	- returns the string until \n and copy to the variable line_2b_printed.
* `ft_keep_rest`	- copy read excess (string after \n) to the static variable so it won't get lost.
* `get_next_line`	- main function that calls for the read, return_line and keep_rest functions and returns line_2b_printed.

**Functions in `get_next_line_utils.c`**

* `ft_strlen`		- find length of string.
* `ft_strjoin`		- concatenate two strings into a new string (with malloc). I added a free function (line 42) to free the first argument.
* `ft_strchr`		- locate character in string (first occurrence).

**Extra on `get_next_line_bonus.c`**

* get_next_line() can manage multiple file descriptors at the same time.
For example, if you can read from the file descriptors 3, 4 and 5, you should be
able to read from a different fd per call without losing the reading thread of each
file descriptor or returning a line from another fd.
