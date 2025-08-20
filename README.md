## ReadME

Here are the files for the **Intro to R** course for the 2025 master's cohort in Political Science at the University of Mannheim. In this course we will use the open-source software `R` and RStudio. Before we get started, we would like you to install both `R` and RStudio on your computer. Here we provide you with detailed instructions to install these programs. If you have any problems getting `R` and RStudio running, do not hesitate to drop us an email.

## What is `R`?

`R` is a programming language designed to help you perform statistical analysis, create graphics, and later on write your own statistical software. `R` is becoming increasingly popular and knowledge of `R` will help you in the job market. `R` is probably the most versatile statistical tool out there (and its free and open source so you can literally use it anywhere).

### How to install `R`

1. Open your browser and go to [https://cran.rstudio.com](https://cran.rstudio.com).
2. Download the latest *release* distribution (4.5.1 as of July 2025) for your operating system (OS):
    - Windows users: Click on *Download R for Windows* and then click on *base*. Click on [Download R 4.5.1 for Windows](https://cran.rstudio.com/bin/windows/base/release.html).
    - Mac users: Click on *Download R for (Mac) OS X* and download [`R-4.5.1.pkg`](https://cran.rstudio.com/bin/macosx/base/R-4.5.1.pkg).
3. Run the installation from the file you just downloaded (`.exe` or `.pkg`).
4. Now that `R` is installed, you need to download and install RStudio.

## RStudio

RStudio is a great graphical user interface for `R` and will be the program which we will use during the lab sessions. In recent years, a growing number of features have been added to this graphical user interface, which makes it the preferred choice for learning `R`, especially among beginners. You can think about it as `R` being the engine of the car and RStudio being the dashboard. 

### How to install RStudio

1. Go to [www.rstudio.com](https://www.rstudio.com) and click on the *Download* button on the top bar.
2. Scroll down and click on the *Download* button for the free RStudio Desktop version.
3. Download the latest version for your operating system:
    - Windows users: Click on the button *Download RStudio for Windows*. The file should have a  `.exe` extension. 
    - Mac users: Click on *Download RStudio for (Mac) OS X*. You should see a `.dmg` extension.
4. Install it!   

### The RStudio graphical user interface (GUI)

The RStudio interface has four panes:

![](images/rstudio_interface.png)

  - **Editor**: This is were you usually code. You can either use .Rmd (R Markdown) or .R (plain R code) files.
  - **Console**: This is where the results appear once you execute your R-code. You can also directly type R-code into the console and execute it. However, we cannot save this code which is why we usually work in the Editor.
  - **Environment**: Here you have an overview over all the objects currently loaded in your environment. You will learn more about objects later in the course.
  - **Files, Plots, Packages, Help, Viewer**: Plots and other things will appear here, don't worry too much about it for the moment.

### RStudio Projects

RStudio projects, `.Rproj`, make it straightforward to divide your work into multiple contexts (Environments), each with its own working directory, workspace, history, and source documents. A project is basically a folder on your computer that holds all the files relevant to a particular piece of work. Working in RStudio Projects has multiple advantages:

  - Once an RStudio Project is set up, you do not have to worry about your working directory anymore.
  - When opening an RStudio Project, a new `R` session (process) is started. This makes sure that things you do in different projects do not mess up or get intermixed. *Note: By default, R projects share the same default library of packages (software addons for the R providing additional or revised functionality). Each version of R (not RStudio or RStudio Project) shares the same local library of installed packages (on the device you are using). To provide isolated libraries and version control, you can employ additional packages (e.g. `renv`) or software (e.g. Docker).*
  - RStudio projects can easily be exported to and imported from GitHub.

## R Markdown

In the “Intro to R” Course, we utilize R Markdown files, `.Rmd`, to combine formatted text (formatted using “Markdown” syntax) and code (incl. results), which can be exported to, among others, `.html` or `.pdf` files. For more details on using `R` Markdown see <http://rmarkdown.rstudio.com>.

### Writing and executing code in R Markdown

In `.Rmd` files, you can execute R-code in so called chunks (see image below). When you click the **Knit** or **Preview** button in `R`, a document will be generated that includes both content, as well as the output of any embedded `R` code chunks within the document.

<p align="center">
  <img width="80%" src="images/chunk.png">
</p>

- To add a chunk, use the shortkey <code>Ctrl + Alt + I</code> (on Windows and Linux). For macOS, use either <code>Cmd + Option + I</code> or <code>Cmd+Alt+I</code>. 
- To run a complete code chunk on Windows and Linux, use <code>Ctrl + Shift + Enter</code> (Windows, Linux). For macOS, use either <code>Cmd + Shift + Enter</code> or <code>Cmd + Option + C</code>. 
- To run parts of your code, you can highlight the respective code and press <code>Ctrl + Enter</code> or <code>Cmd + Enter</code> respectively. To run a single line of code, select the line with your cursor and press the same shortcuts used to run highlighted parts of code.

### Chunk Options

Chunk output in your final document can be customized with knitr options, arguments set in the `{}` of a chunk header. Here are some useful arguments:

  - `include = FALSE` prevents code and results from appearing in the finished file. R Markdown still runs the code in the chunk, and the results can be used by other chunks.
  - `echo = FALSE` prevents code, but not the results from appearing in the finished file. This is a useful way to embed figures.
  - `message = FALSE` prevents messages that are generated by code from appearing in the finished file.
  - `warning = FALSE` prevents warnings that are generated by code from appearing in the finished.
  - `fig.cap = "..."` adds a caption to graphical results.

### Cheatsheet

For formatting and an overview of additional R Markdown functionalities, we recommend the [R Markdown Cheat Sheet](https://raw.githubusercontent.com/rstudio/cheatsheets/main/rmarkdown-2.0.pdf).

---

## Replication of results with set.seed

Setting seeds is extremely helpful for replicability. It allows you to reproduce your results, e.g. a random draw, so that whenever you execute a script again, the random draw is exactly the same as before. A random draw could be sampling values (e.g. drawing 1000 observations from 10000 observations) or generating random values (e.g. ten numbers from 1-100).

To do so, use the command `set.seed()` and define an integer value as the "seed", e.g. `set.seed(2025)`.
