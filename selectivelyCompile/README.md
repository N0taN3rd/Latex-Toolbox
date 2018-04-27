The [subfile]({http://ftp.math.purdue.edu/mirrors/ctan.org/macros/latex/contrib/subfiles/subfiles.pdf) package is a much more efficient way to bring in the sub parts of a large latex document.

Each part of the complete document that is split up into its own text file brought is added to the document from the main tex file via  
```tex
\subfile{file} 
```

Each subfile has the following structure
```tex
\documentclass[main.tex]{subfiles}
\begin{document}
% content
\end{document}
```

And each subfile has access to all packages included in the preable of the main document.

I think there is an package option for subfiles that allows each subfile to use its own preamble. 

Best pratice I found is include everything used by your subfiles in the main tex files preamble

Particulars as to the setup and macros documented as comments in the main.tex file included in this gist

***The wrapping of figures, tables is optional!! And is only included in this MWE as an example as to what can be done using this approach***

***It only required portion of the MWE is the setup shown in main.tex*** 
