---
title: "Workshop Examples"  
author: "Melissa Monk"
date: ''
output:
  pdf_document:
    fig_caption: yes    
    includes:
      in_header: header.tex
    keep_tex: yes
    number_sections: yes
    toc: yes
    toc_depth: 4
documentclass: article
fontsize: 12pt
geometry: margin=1in
csl: CJFAS.csl
bibliography: BibFile.bib
link-citations: yes
---



Change some of the YAML settings to see what happens.

Notice, the down arrow at line 22.  If you click this, you can hide the R code chunk.  This is helpful when working through a large document.

On the right side of the R code chunk are additional options, Settings, a down arrow (run previous R code chunks), and a green play button (runs the current chunk).  It's handy to check R code chunks as you go and to debug.  Within the Assessment template, this is also the only way to see variables in your Environment. 



# Epmhasis (R markdown and LaTeX)

*Sebastes*

\emph{Sebastes}

\textit{Sebastes}


# Headers

## Subhead 2

### Subhead 3

#### Subhead 4



# Commenting

<!-- comment here -->



# Links

[Github](www.github.com)


# Lists

R Markdown are finicky with spacing...
* Item 1
* Item 2
    + Item 2a
    + Item 2b


 * Item 1
 * Item 2
    + Item 2a
    + Item 2b



Bulleted list

\begin{itemize}[noitemsep,nolistsep,topsep=0pt]

\item \href{https://git-scm.com/book/en/v2/Getting-Started-Installing-Git}{Git}

\item \href{https://cran.r-project.org/bin/windows/base/}{R}

\end{itemize}



<!--
Numbered list
\begin{enumerate}[noitemsep,nolistsep,topsep=0pt]

\item \href{https://git-scm.com/book/en/v2/Getting-Started-Installing-Git}{Git}

\item \href{https://cran.r-project.org/bin/windows/base/}{R} 

\end{enumerate}
-->

# References and Citations

We can reference a document section, see Lists in Section \ref{lists}.

Citations: [@Love2002; @Love2002]

Love [-@Love2002]


#Figure from a file
You can use any file extension, including PDFs

![Here's my caption \label{fig:fig_example}](RMarkdownFLow.png)

Figures are referenced using LaTeX syntax \ref{fig:fig_example}.

Put a space between the ] and ( above. Knit the document.  


Now try adding your own picture to the directory, adding it in here, and referencing it.



# R code chunks

You can embed an R code chunk like this:




Play witht the r code chunk options, echo=TRUE, include=FALSE, results='asis'





# Figure from R code chunk

You can also embed plots, for example:



Note, you need extra \\s when using LaTeX syntax within an R code chunk, or when inserting a backslash in R markdown.  The same goes with percent signs and any other LaTeX reserved symbol.



<!--
We can now reference Figure \ref{fig:pressure}.  Note where this text ends up.

Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.

-->


#Tables





Try changing the R chunk options above. 

We can now reference Table \ref{tab:Table_example}.

Now, try putting the R code chunk within and HTML comment.



# Create you own table
Either create a .csv file or copy one into the repo folder on your computer.

Now, create a table!




#Math mode
 <!--
You can use LaTeX math mode both inline and for inserting equations. It's handy for using inline math mode for management measure and lat/long.

Inline looks like this:  $SPR_{40\%}$  
*Note the % sign has a \ when used in math mode, but not in R markdown text.

To get degrees and minutes type: $40^\circ 10^\prime$   

-->

#References

