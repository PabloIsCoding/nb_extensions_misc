# Nbextensions Misc

This is just a personal "repo". It's really just a bunch of notes on how to set up jupyter notebook extensions that I find most useful. 

## How to install nbextensions

```
conda install -c conda-forge jupyter_contrib_nbextensions
```

(https://jupyter-contrib-nbextensions.readthedocs.io/en/latest/install.html)

## Useful extensions

* Collapsible Headings
* Equation Auto Numbering
* ExecuteTime
* Nbextensions edit menu item
* Freeze
* Move selected cells
* Scratchpad
* Autopep8
* Notify
* ScrollDown
* Snippets
* Table of Contents (2)
* Variable Inspector

## How to set up snippets

There is a file: `.....\anaconda3\envs\some_env\share\jupyter\nbextensions\snippets\snippets.json`

You put there something like this

```JSON
{
    "snippets" : [
        {
            "name": "np, pd, plt, sns",
            "code": [
                "import numpy as np",
                "import pandas as pd",
                "import matplotlib.pyplot as plt",
                "import seaborn as sns",
                "plt.style.use('fivethirtyeight')",
                "plt.rcParams['figure.figsize'] = (18, 10)"
            ]
        }
    ]
}
```

There is a `snippets.json` file in this repo too.