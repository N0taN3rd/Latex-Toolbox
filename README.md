# Latex Toolbox
Useful Latex macros / setup for grad students derived from my masters thesis.

The choice of packages and macros included/recommended by this repo has one goal in mind:

**Make writing a large LaTex document as simple and configurable as possible while producing a beautiful looking document.**


# Whats included

Additional documentation found in each file  

#### Selectively Compile Directory
Minimal Working Example of the selective compile setup I used in my MS thesis

#### algorithmUtil.sty
Macros and setup I found to be useful when typesetting algorithms
- `for each` loop
- macros for typesetting pseudo code

Package options
- **topSpace**: length unit string indicating how much space to use for `\algoTopSpace` macro
- **disable**: boolean flag to indicating that the space added by the `\algoTopSpace` macro should not be applied. `\algoTopSpace` macro still exists but does not add space
- **smallerText**: boolean flag indicating the font size of the `algorithmic` environment should be `\footnotesize`


#### generalUtil.sty
Small collection of useful macros I have written for
- Better justification of `\texttt`
- Bold blue, brown, red, text
- An edit footnote that is number separately and has a different symbol
- Macro to tighten up the spacing between list environment items  

#### graphicsUtil.sty
Collection of useful macros that wrap `\includegraphics`
- Graphics manipulation while keeping the graphics aspect ratio
- Macros combining `\centering` and `\ContinuedFloat`  
- Macros for adding additional padding to space about `figure` environments

Optional package options
- **topSpace**:  length unit string indicating how much space to use for `\figureTopSpace` macro
- **doubleTopSpace**: length unit string indicating how much (2x) space to use for `\figureTopDoubleSpace` macro
- **disable**: boolean flag to indicating that the space added by the `\figureTopSpace` and `\figureTopDoubleSpace` macros should not be applied. Macro still exists but do not add space


#### mintedUtil.sty
Collection of useful macros for the `minted` package
- Reduce space after minted environments but before `\caption`
- Macros for minting: HTML, JS, CSS, Java, Python, HTTP, Bash, JSON
- Macros for inline minting: HTML, JS, CSS


#### tableUtil.sty
- Macro for per table changes to `\arraystretch`
- Macros for adding space above a table

Optional package options
- **topSpace**:  length unit string indicating how much space to use for `\tableTopSpace` macro
- **doubleTopSpace**: length unit string indicating how much (2x) space to use for `\tableTopDoubleSpace` macro
- **disable**: boolean flag to indicating that the space added by the `\tableTopSpace` and `\tableTopDoubleSpace` macros should not be applied. Macro still exists but do not add space

#### urlUtil.sty
- Adjusts `biburllcpenalty` and `biburlucpenalty` to ensure URLs do not escape margins
- Adds additional URL breaks used when the `breaklinks` option is used with the `hyperref` package
- Macro to include non-hyperlinked URLs in text that break (line wrap) easily
- Macro to add a hyperlinked URL as a footnote


#### recommendedPackages.sty
Opinionated package recommendation (in proper load order) featuring:
- Typography improvements
- Math mode / symbol improvements
- Source code syntax highlighting
- Easy quotes
- Improved bibliography management
- Algorithm typesetting
- Easy captioning and subfigures
- Pretty tables
- Simple referencing and URL handling


#### IEETransactionsNetworkingJournalModel.sty
Old Dominion University [requires](https://www.odu.edu/content/dam/odu/offices/graduate-studies/thesis-dissertation/docs/thesis_dissertation_guide.pdf) a journal model to be followed for citation, figure/table caption styling.

This style file will configure your latex document, in combination with the  [oduwsdl/wsdlthesis](https://github.com/oduwsdl/wsdlthesis) document class, to conform to the IEE Transactions Networking journal style.
