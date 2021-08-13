# Jupyter

*Notebook* files have the extension `.ipynb` to distinguish them from plain-text Python programs. The notebook file is stored in a format called JSON, which allows Jupyter to mix source code, text, and images, all in one file.

Jupyter mixes code and text in different types of blocks, called *cell*s. We often use the term *code* to mean “the source code of software written in a language such as Python”. A *code cell* in a Notebook is a cell that contains software; a *text cell* is one that contains ordinary prose written for human beings.

Notebooks can also render *Markdown* - a simple plain-text format for writing lists, links, and other things that might go into a web page. Turn the current cell into a Markdown cell by entering the Command mode (`Esc`/gray) and press the `M` key. `In []:` will disappear to show it is no longer a code cell and you will be able to write in Markdown.

```
{
  "cells": [
　　  {
       "cell_type": "markdown",
       "id": "b29191bf-5df7-471c-b8c9-5d1b6e9a29bf",
       "metadata": {},
       "source": [
         "Download the latest [Miniforge ...",
         "\n",
         "```\n",
         "$ bash Miniforge3-Linux-aarch64.sh\n",
         "(base) ~$ conda install pandas\n",
         "(base) ~$ conda install matplotlib\n",
         "(base) ~$ conda install jupyterlab\n",
         "(base) ~$ conda install scipy\n",
         "```"
       ]
    },
    {
      "cell_type": "code",
      "execution_count": 1,
      "id": "7a222d09-cf43-44f7-b3ad-409de41e8503",
      "metadata": {},
      "outputs": [
        {
          "name": "stdout",
          "output_type": "stream",
          "text": [
            "54\n"
          ]
        }
      ],
      "source": [
        "x = 6 * 7 + 12\n",
        "print(x)"
      ]
    },
    ...
```

Standard Markdown (such as we’re using for these notes) won’t render equations, but the Notebook will. Create a new Markdown cell and enter the following:

```
$\sum_{i=1}^{N} 2^{-i} \approx 1$
```

The notebook shows the equation as it would be rendered from *LaTeX* equation syntax. The dollar sign, `$`, is used to tell Markdown that the text in between is a LaTeX equation. If you’re not familiar with LaTeX, underscore, `_`, is used for subscripts and circumflex, `^`, is used for superscripts. A pair of curly braces, `{` and `}`, is used to group text together so that the statement `i=1` becomes the subscript and `N` becomes the superscript. Similarly, `-i` is in curly braces to make the whole statement the superscript for `2`. `\sum` and `\approx` are LaTeX commands for “sum over” and “approximate” symbols.
