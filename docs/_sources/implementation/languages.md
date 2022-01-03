# Programming Languages

:::{panels}
:container: text-center

**[C](#c)**
^^^
[Getting started with embedded C](#c)
---

**[Python](#python)**
^^^
[Installation and getting started](#python)
---

**[Julia](#julia)**
^^^
[Installation and getting started](#julia)
---

**[MATLAB](#matlab)**
^^^
[Installation and getting started](#matlab)

:::

DSP theory and algorithms can be studied from a purely mathematical 
perspective with minimal computing or programming background. However, a more 
holistic perspective acknowledges tradeoffs between signal quality and 
implementation complexity. 

Although some DSP systems are implemented in assembly or hardware description 
languages, it is more common to use a low level programming language like C. 
high level languages are often used for prototyping and simulation of DSP 
algorithms.

If you are not comfortable with programming, don't worry! Computing and DSP 
are complementary; a great way to demystify DSP algorithms is by implementing 
them in software, and great way to learn software design patterns is by 
implementing DSP algorithms.

In this course, we will develop the embedded implementation in [C](#c). 
Prototyping and simulation can be done using either 
[Julia](#julia), [Python](#python), or [MATLAB](#matlab).

## Popular languages for DSP

A variety of sources have tracked the popularity of programming languages over 
time, usually in the form of developer surveys.

* [IEEE combined ranking][ieee]
* [Annual stack overflow surveys][stack]
* [Popularity on GitHub][octoverse]
* [TIOBE index][tiobe]

[octoverse]:https://octoverse.github.com
[stack]:https://insights.stackoverflow.com/survey/
[ieee]:https://spectrum.ieee.org/top-programming-languages/
[tiobe]:https://www.tiobe.com/tiobe-index/

## Package management

Many of the most frustrating aspects of programming and software development can be avoided by using a [package manager](https://en.wikipedia.org/wiki/Package_manager), both for your operating system and for your particular language.

* On Windows, the [package manager](https://docs.microsoft.com/en-us/windows/package-manager/) can be accessed using the `winget` command in [powershell](https://aka.ms/terminal).

* Mac OS, [Homebrew](https://brew.sh) is the most popular package manager.

* Python's package manager [pip](https://pypi.org/project/pip/) is a standalone program which can be accessed using either the command `pip` or `pip3` depending on your installation.

* Julia's package manager [Pkg](https://docs.julialang.org/en/v1/stdlib/Pkg/) can be accessed by pressing the `]` key in the Julia REPL

## Jupyter

Interactive programming can be extremely helpful for simulation and prototyping. [Project Jupyter](https://jupyter.org) (portmanteau of Julia, Python, R) allows for several languages to be developed interactively using notebooks.

The easiest way to get started is by first installing [Python](#Python) and then using pip to install [Jupyter Lab](https://jupyterlab.readthedocs.io/)

```console
pip install jupyterlab
```

Then, you can run it using the `jupyter-lab` command.

# C

The C programming language has consistently ranked among the top languages for 
decades. Currently, C is popular for embedded systems, operating systems, and 
high performance/supercomputer applications.

**Getting started with C for embedded systems**

* [Setup guide for STM32 discovery board](https://danjacobellis.net/EE445S-lab/stm32h735g.html)
* [Real-time DSP Lab #1](https://danjacobellis.net/EE445S-lab/lab1/index.html)


# Python

Python is currently the most popular general purpose programming language.
Use in embedded and real-time systems is possible via [micropython](https://micropython.org).

**Installation and getting started**

You can install Python 3 using your operating system's [package manager](#package-management).

```console
winget install Python.Python.3
```

* [Homebrew and python](https://docs.brew.sh/Homebrew-and-Python)
    
```{warning}
Many operating systems will have Python 2 pre-installed. Depending on your operating system and installation process, the `python` and `pip` commands might point to Python 2 while `python3` and `pip3` commands point the python 3. You may want to create or modify any [symbolic links](https://en.wikipedia.org/wiki/Symbolic_link) to the `python` and `pip` commands after installation to avoid confusion or modify path [environemt variables](https://en.wikipedia.org/wiki/Environment_variable)
```

A great way to write Python code for simulation and prototyping is with [Jupyter Lab](#Jupyter).

# Julia

Julia is one of the fastest growing languages. It is increasingly used in
education and industry, especially for high-performance computing and 
machine learning applications.

**Installation and getting started**

You can install Julia using your operating system's [package manager](#package-management).

```console
winget install Julialang.Julia
```

```console
brew install --cask julia
```
    
```{note}
The official Julia language organization also provides [installers](https://julialang.org/downloads/), platform-specific [installation instructions](https://julialang.org/downloads/platform/), and several [tutorials](https://julialang.org/learning/).
```

# MATLAB

MATLAB is commercial software. Many textbooks, especially in the field of 
signal processing, use MATLAB since it offers a set of interoperable, 
application-specific toolboxes for everything from filter design to
embedded code generation.

**Installation and getting started**

* [Licence and installation instructions for UT Austin students](https://ut.service-now.com/sp?id=ut_bs_service_detail&sys_id=f9d65c7c4ff9d200f6897bcd0210c77d)


