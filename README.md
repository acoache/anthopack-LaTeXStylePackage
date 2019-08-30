## LaTeX style package


This LaTeX style package contains many commands that are useful when writing mathematics in TeX (.tex) files. It is still a work in progress, do not hesitate to contribute by adding commands or raising issues related to the package!

## Location of your own style packages

The main advantage of such package is that correctly placed, it can be made available to all other TeX files you create without copying the .sty file in the same folder. The package can be loaded by adding in any TeX file the line

```tex
% Load custom package
\usepackage{anthopack_LaTeX}
```

The procedure to do so using MiKTeX is based on [xport's answer to this StackExchange question](https://tex.stackexchange.com/questions/1137/where-do-i-place-my-own-sty-or-cls-files-to-make-them-available-to-all-my-te/20121):


* Create a path of the form `C:\...\NameFolder\tex\latex`.
* Place your own packages in subdirectories.
* Open `MiKTeX Setting (Admin)`, select `Roots` tab and add your path `C:\...\NameFolder`. Note that the trailing `\tex\latex` with any subdirectory must not be included.
* Select `General` tab and press the `Refresh FNDB` button.


## Packages


Uncommented `\RequirePackage` commands are required to support all commands in the package. All other commented packages are commonly used packages with a small description. You can either uncomment them if you want to always load these packages or refer to them before loading a package.



## French and English keywords


If you create a TeX file with the command

```tex
\usepackage[french]{babel}
```

it basically means you are writing in French. Thus this package automatically writes environment names in French and loads the following packages for accented characters:

```tex
\usepackage[utf8]{inputenc}
\usepackage[T1]{fontenc}
```

Otherwise, environment names are written in English.


## Mathematics commands

All commands are explained and an example of appropriate use in a TeX file is provided for each one of them. 


### Authors


- Anthony Coache *(creator, author)*