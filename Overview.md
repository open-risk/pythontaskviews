![Visual of Jupiter's Moons](Jupyter.png "Overview of the Jupyter Universe")


Overview of the **Ju**lia-**Py**thon-**R** Universe
---------------------------------------------------

A side-by-side review of the main open source ecosystems supporting the [Data Science](Data%20Science "wikilink") domain: Julia, Python, R, sometimes abbreviated as *Jupyter*.

### Motivation

A large component of [Quantitative Risk Management](Quantitative%20Risk%20Management "wikilink") relies on data processing and quantitative tools (aka [Data Science](Data%20Science "wikilink")). In recent years [open source](:Category:Open%20Source "wikilink") software targeting Data Science finds increased adoption in diverse applications. The **Overview of the Julia-Python-R Universe** article is a side by side comparison of a wide range of aspects of Python, Julia and R language ecosystems. The comparison of the three ecosystems aims:

-   To be useful for people that are somewhat familiar with programming and want to inspect options and use the most appropriate tool
-   To promote interoperability, cross-validation and overall best-practices
-   To be factual as much as possible without drifting to judgement / opinions
-   To cover use cases relevant for the implementation of quantitative risk models

The comparison **does not** aim:

-   To be a detailed / comprehensive catalog of *all* available libraries (which count to many thousands!)
-   To cover use cases very removed from quantitative risk models
-   To be totally exhaustive (e.g to identify all the possible computer systems one can run a Python interpreter on, or count all the possible ways one can perform linear regression in R)

### Disclaimers

The comparison does absolutely not provide an assessment of which system is "better". The proper way to use the comparison is to start with one's objectives, knowledge level, use case.

The comparison attempted here is not entirely appropriate as the three systems have quite different origins and architectural design choices. For example, strictly speaking R is not a *general* programming language. R is a system for statistical computation and graphics. It consists of a sufficiently general language plus a run-time environment with graphics, a debugger, access to certain system functions, and the ability to run programs stored in script files. Yet despite the disclaimer a comparison *is* justified because in very large domain of applications and use cases the three frameworks can be used interchangeably (or nearly so)

### Structure

The comparison data are provided in tabular format in several distinct tables. Each table documents a relevant language or ecosystem subdomain. The number and focus areas of the different table are somewhat arbitrary and may expand in the future. The order is roughly from more generic aspects towards more specialized / advanced areas, concluding with interoperatibility.

Each table entry (row) highlights key functionality within the subdomain. The language columns point to information or packages and (where applicable) there is commentary. Reference links are included when useful.

At the bottom of some tables there is a row indicated *Package Review*. This row has a collection of links to the *CRAN Task Reviews* that aim to summarize the large number of R packages available for some data science tasks. *There are also links to a mirror effort to create [Python Task Views](https://www.pythondatascience.org/) (this content is still WIP - contributors welcome, see below)*

### Getting Involved

You can provide simple and anonymous feedback on the [wiki version of the overview](https://www.openriskmanual.org/wiki/Overview_of_the_Julia-Python-R_Universe) using the feedback button at the bottom of the page. Alternatively you can become an Open Risk Manual author and actively edit the page. If you are more comfortable using github / markdown, there is a [mirror page available here](https://github.com/open-risk/pythontaskviews/blob/master/Overview.md). Please note that the tables are in html format as they are generated automatically.

People interested in developing the [Python Task Views](https://www.pythondatascience.org/) can do so via [the github repo](https://github.com/open-risk/pythontaskviews).

History and Community
---------------------

The objective of this section is to provide an overall comparison of the history of the two ecosystems, towards answering the question: who is really behind Python, R and Julia?

<table>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<thead>
<tr class="header">
<th align="left"><p>Aspect</p></th>
<th align="left"><p>Python</p></th>
<th align="left"><p>R</p></th>
<th align="left"><p>Julia</p></th>
<th align="left"><p>Comment</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>First Release</p></td>
<td align="left"><p>1991</p></td>
<td align="left"><p>1995</p></td>
<td align="left"><p>2009</p></td>
<td align="left"><p>Both the Python and R ecosystems have a long history of development and both received a lot of attention in the last few years as open source data science became more widerspread. Julia is relatively more recent</p></td>
</tr>
<tr class="even">
<td align="left"><p>Initial Authors</p></td>
<td align="left"><p>Guido van Rossum</p></td>
<td align="left"><p>Ross Ihaka and Robert Gentleman</p></td>
<td align="left"><p>Jeff Bezanson, Stefan Karpinski, Viral B. Shah, and Alan Edelman</p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>Current Stable Version</p></td>
<td align="left"><p>3.7</p></td>
<td align="left"><p>3.5</p></td>
<td align="left"><p>1.2</p></td>
<td align="left"><p><a href="https://www.python.org/downloads/">Check here for Python</a>, <a href="https://www.r-project.org/">Check here for R</a>, <a href="https://julialang.org/downloads/">Check here for Julia</a></p></td>
</tr>
<tr class="even">
<td align="left"><p>Current Governance</p></td>
<td align="left"><p><a href="https://www.python.org/psf/">Python Software Foundation</a> (Non Profit)</p></td>
<td align="left"><p><a href="https://www.r-project.org/foundation/">R Foundation</a> (Non Profit)</p></td>
<td align="left"><p><a href="https://julialang.org/blog/2019/02/julia-entities">Julia Governance Overview</a></p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>Open Source License</p></td>
<td align="left"><p><a href="https://docs.python.org/3/license.html">PSF License</a></p></td>
<td align="left"><p><a href="https://www.gnu.org/licenses/gpl-3.0.en.html">GNU General Public License</a></p></td>
<td align="left"><p><a href="https://github.com/JuliaLang/julia/blob/master/LICENSE.md">MIT License</a></p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Size of Core Contributors</p></td>
<td align="left"><p>2-90 depending on definition</p></td>
<td align="left"><p><a href="https://www.r-project.org/contributors.html">20</a></p></td>
<td align="left"></td>
<td align="left"><p>Python Core Team Size is difficult to establish (e.g. full-time / part-time, activity level) and there is no single authoritative source, Similarly for Julia</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Size of Broader Developer Communities</p></td>
<td align="left"><p>Third most popular in number of repositories and number of contributors</p></td>
<td align="left"><p>Not in Top 10 of community size</p></td>
<td align="left"><p>Not in Top 10 of community size</p></td>
<td align="left"><p>Note: R programmers might not necessarily self-identify as <em>developers</em> (but as data scientists, statisticians etc.)</p></td>
</tr>
<tr class="even">
<td align="left"><p>Developer Associations</p></td>
<td align="left"><p><a href="https://uk.python.org/">UK Python Association</a>, <a href="https://www.pyladies.com/">pyLadies</a></p></td>
<td align="left"><p><a href="https://rladies.org/">R-Ladies</a></p></td>
<td align="left"></td>
<td align="left"><p>Formally organized associations promoting Python, R or Julia</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Important Non-Profit Sponsors</p></td>
<td align="left"><p><a href="https://numfocus.org/">Numfocus</a></p></td>
<td align="left"><p><a href="https://www.bioconductor.org/">Bioconductor</a></p></td>
<td align="left"><p><a href="https://numfocus.org/">Numfocus</a></p></td>
<td align="left"><p>A number non-profit organizations support these open source ecosystems explicitly or implicitly</p></td>
</tr>
<tr class="even">
<td align="left"><p>Important Corporate Sponsors</p></td>
<td align="left"><p>Diverse</p></td>
<td align="left"><p>Diverse</p></td>
<td align="left"><p><a href="https://juliacomputing.com/">Julia Computing, Inc.</a></p></td>
<td align="left"><p>Commercial sponsors may be supporting these ecosystems explicitly or implicitly</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Important Conferences</p></td>
<td align="left"><p><a href="https://pycon.org/">pycon</a>, <a href="https://www.europython-society.org/">europython</a></p></td>
<td align="left"><p><a href="https://www.r-project.org/conferences/">useR!</a></p></td>
<td align="left"><p><a href="https://juliacon.org">Juliacon</a></p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Important Journals</p></td>
<td align="left"></td>
<td align="left"><p><a href="https://journal.r-project.org/">The R Journal</a></p></td>
<td align="left"></td>
<td align="left"><p><a href="https://joss.theoj.org/">Journal of Open Source Software</a>, <a href="https://paperswithcode.com/">Papers with Code</a> covering all three systems</p></td>
</tr>
<tr class="odd">
<td align="left"><p>IRC Channels</p></td>
<td align="left"><p>#python</p></td>
<td align="left"></td>
<td align="left"><p>#julia</p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Reddit</p></td>
<td align="left"><p><a href="https://www.reddit.com/r/Python/">Python subreddit, 428k members</a></p></td>
<td align="left"><p><a href="https://www.reddit.com/r/rstats/">R Stats subreddit, 30k members</a></p></td>
<td align="left"><p><a href="https://www.reddit.com/r/Julia/">Julia subreddit, 8k members</a></p></td>
<td align="left"><p><a href="https://www.reddit.com/r/datascience/">Data Science subreddit (discussing Python, R and Julia topics)</a></p></td>
</tr>
<tr class="odd">
<td align="left"><p>Online Forums and Blogs</p></td>
<td align="left"><p>Too many</p></td>
<td align="left"><p>Too many</p></td>
<td align="left"></td>
<td align="left"><p>The Python and R ecosystems have an extensive numbers of blogs, forums etc. (with varying level of quality)</p></td>
</tr>
</tbody>
</table>

Devices and Operating Systems
-----------------------------

This section aims to answer the question: Where (as in what kind of device and operating system) can I use Python, R or Julia? *NB: This is not a how-to install Python or R in your system!*, just an overview of what is available where.

<table>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<thead>
<tr class="header">
<th align="left"><p>Aspect</p></th>
<th align="left"><p>Python</p></th>
<th align="left"><p>R</p></th>
<th align="left"><p>Julia</p></th>
<th align="left"><p>Comment</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Linux Desktop</p></td>
<td align="left"><p>Comes pre-installed</p></td>
<td align="left"><p>apt-get install r-base</p></td>
<td align="left"><p>apt-get install julia / Linux installer file</p></td>
<td align="left"><p>Python is generally pre-installed as it is used by the Linux system itself. Different distributions may include different (potentially very old) versions of the three languages.</p></td>
</tr>
<tr class="even">
<td align="left"><p>Windows</p></td>
<td align="left"><p><a href="https://www.python.org/downloads/windows/">Windows installer</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/bin/windows/base/">Windows installer</a></p></td>
<td align="left"><p><a href="https://julialang.org/downloads/platform.html#windows">Windows installer</a></p></td>
<td align="left"><p>All three languages are available for both Windows 7 and Windows 10 and 32 bit / 64 bit.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>MacOS</p></td>
<td align="left"><p>2.7 version is pre-installed</p></td>
<td align="left"><p>MacOS installer</p></td>
<td align="left"><p>MacOS installer file</p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Raspbian</p></td>
<td align="left"><p>Pre-installed</p></td>
<td align="left"><p>apt-get install r-base</p></td>
<td align="left"><p>apt-get install julia</p></td>
<td align="left"><p>Linux is the operating system of choice for IoT devices, which means a basic Python installation is generally available</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Android / iOS</p></td>
<td align="left"><p>Via <a href="https://pypi.org/project/python-for-android/">python-for-android</a></p></td>
<td align="left"><p>No</p></td>
<td align="left"><p>No</p></td>
<td align="left"><p>Python, R or Julia are not readily integrated on mobile devices (see also Deployment entry). Check <a href="https://github.com/termux/">Termux</a> for an alternative option</p></td>
</tr>
<tr class="even">
<td align="left"><p>iOS</p></td>
<td align="left"><p>No</p></td>
<td align="left"><p>No</p></td>
<td align="left"><p>No</p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>Cloud Servers</p></td>
<td align="left"><p>As per Linux Desktop above</p></td>
<td align="left"><p>As per Linux Desktop above</p></td>
<td align="left"><p>As per Linux Desktop above</p></td>
<td align="left"><p>Cloud servers typically run the Linux operating system and have Python installations available</p></td>
</tr>
</tbody>
</table>

Package Management
------------------

This section aims to answer the question: How can I extend the Python, R or Julia functionality with existing libraries. The ease of finding and installing packages is a very important aspect of the popularity of both and in marked contrast e.g. to languages like C++

<table>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<thead>
<tr class="header">
<th align="left"><p>Aspect</p></th>
<th align="left"><p>Python</p></th>
<th align="left"><p>R</p></th>
<th align="left"><p>Julia</p></th>
<th align="left"><p>Comment</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Discovery of Packages</p></td>
<td align="left"><p>Online Search, Built-in PyCharm access to <a href="https://pypi.org/">PyPI</a></p></td>
<td align="left"><p>R-Studio Built-in access to <a href="https://cran.r-project.org/">CRAN</a></p></td>
<td align="left"><p><a href="https://pkg.julialang.org/docs/">Julia Docs</a>, <a href="https://juliaobserver.com/packages">Julia Observer</a></p></td>
<td align="left"><p>Python packages are released on PyPI, R packages are released on CRAN</p></td>
</tr>
<tr class="even">
<td align="left"><p>Number of Packages (Oct 2019)</p></td>
<td align="left"><p>199,816</p></td>
<td align="left"><p>15102</p></td>
<td align="left"><p>~2496</p></td>
<td align="left"><p>Check here for the latest count: <a href="https://pypi.org/">Python</a>, <a href="https://cran.r-project.org/web/packages/">R</a>, <a href="https://github.com/JuliaRegistries/General/blob/master/Registry.toml">Julia</a></p></td>
</tr>
<tr class="odd">
<td align="left"><p>Online Repositories</p></td>
<td align="left"><p>PyPI, via linux distributions</p></td>
<td align="left"><p>CRAN</p></td>
<td align="left"></td>
<td align="left"><p>github, gitlab, bitbucket etc are used for releasing Python, R and Julia for open source packages online, coordination of development and other community support</p></td>
</tr>
<tr class="even">
<td align="left"><p>Package Installation</p></td>
<td align="left"><p>Done at OS level (PyPI, setup, <a href="https://conda.io/en/latest/">conda</a>, pip, easy_install, apt)</p></td>
<td align="left"><p>Built-in install.packages</p></td>
<td align="left"><p>Built-in Pkg package manager</p></td>
<td align="left"><p>Python installation methods are quite varied (and have evolved over time) and can be either system wide (e.g. a linux distro package) or user specific</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Dependency Management</p></td>
<td align="left"><p>pip, <a href="https://virtualenv.pypa.io/en/stable/">virtualenv</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/packrat/index.html">packrat</a></p></td>
<td align="left"><p><a href="https://docs.julialang.org/en/v1/manual/code-loading/#Federation-of-packages-1">Federated package management</a></p></td>
<td align="left"><p>virtualenv enables using isolated Python distributions and package collections within the same system. Julia uses <em>project environments</em></p></td>
</tr>
<tr class="even">
<td align="left"><p>Loading Packages</p></td>
<td align="left"><p>import statement</p></td>
<td align="left"><p>library statement</p></td>
<td align="left"><p>import / using statements</p></td>
<td align="left"></td>
</tr>
</tbody>
</table>

Package Documentation
---------------------

This section aims to answer the question: How can I document a Python, R or Julia module? The ease and quality of documentation is an important factor in adoption and efficient use of a language as it both helps beginners learn new functionality and experienced users ensure better quality work

<table>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<thead>
<tr class="header">
<th align="left"><p>Aspect</p></th>
<th align="left"><p>Python</p></th>
<th align="left"><p>R</p></th>
<th align="left"><p>Julia</p></th>
<th align="left"><p>Comment</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Source level documentation</p></td>
<td align="left"><p>Built-in docstrings</p></td>
<td align="left"><p>Docstrings</p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/docstring/index.html">docstrings</a></p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Formats</p></td>
<td align="left"><p><a href="https://www.markdownguide.org/">markdown</a>, <a href="http://docutils.sourceforge.net/rst.html">reStructuredText</a></p></td>
<td align="left"><p>markdown, <a href="https://www.latex-project.org/">latex</a></p></td>
<td align="left"><p>Markdown</p></td>
<td align="left"><p>R packages in CRAN include References Manuals (PDF, typically from latex)</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Documentation Generator</p></td>
<td align="left"><p><a href="http://www.sphinx-doc.org/en/master/">sphinx</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/roxygen2/vignettes/roxygen2.html">roxygen2</a></p></td>
<td align="left"><p><a href="https://github.com/JuliaDocs/Documenter.jl">Documenter</a></p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Online documentation</p></td>
<td align="left"><p><a href="https://readthedocs.org/">readthedocs</a></p></td>
<td align="left"><p>CRAN, <a href="https://bookdown.org/">bookdown</a></p></td>
<td align="left"><p><a href="https://pkg.julialang.org/docs/">Julia Docs</a></p></td>
<td align="left"></td>
</tr>
</tbody>
</table>

Language Characteristics
------------------------

This section aims to answer the question: What does code in Python, R or Julia look like from a programming perspective? Many standard aspects of programming languages are available in all three systems so are not included.

<table>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<thead>
<tr class="header">
<th align="left"><p>Aspect</p></th>
<th align="left"><p>Python</p></th>
<th align="left"><p>R</p></th>
<th align="left"><p>Julia</p></th>
<th align="left"><p>Comment</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Compiled / Interpreted</p></td>
<td align="left"><p>Interpreted</p></td>
<td align="left"><p>Interpreted</p></td>
<td align="left"><p>Compiled Just-in-time (JIT)</p></td>
<td align="left"><p>Julia code can be executed interactively</p></td>
</tr>
<tr class="even">
<td align="left"><p>Main Implementation Language</p></td>
<td align="left"><p>C (CPython)</p></td>
<td align="left"><p>C and Fortran</p></td>
<td align="left"><p>Julia</p></td>
<td align="left"><p>This is the language used for the interpretation of a Python or R script. Julia is written in Julia</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Other Implementation Languages</p></td>
<td align="left"><p>Java (<a href="https://www.jython.org/">Jython</a>), <a href="https://github.com/RustPython/RustPython">RustPython</a> etc</p></td>
<td align="left"><p><a href="http://www.pqr-project.org/">pqR</a>, <a href="https://www.renjin.org/">Renjin</a>, <a href="https://bitbucket.org/allr/fastr/src/default/">FastR</a> etc</p></td>
<td align="left"></td>
<td align="left"><p>Many alternative implementations of the underlying interpreter exist for both Python and R. A new approach available for Python and Julia is to compile to <a href="https://webassembly.org/">Webassembly</a> for native execution in the browser: <a href="https://github.com/iodide-project/pyodide">Python/Pyodide</a>, <a href="https://github.com/MikeInnes/Charlotte.jl">Julia/Charlotte</a></p></td>
</tr>
<tr class="even">
<td align="left"><p>Type System</p></td>
<td align="left"><p>Dynamic (Duck) Typing</p></td>
<td align="left"><p>Dynamic</p></td>
<td align="left"><p>Dynamic (Duck) Typing</p></td>
<td align="left"><p>All three systems have essentially dynamic <a href="wikipedia:Type%20system" title="wikilink">type systems</a> (in contrast with languages such as C++, Java or Rust)</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Primitive Data Types</p></td>
<td align="left"><p>Numbers (Integers, Float), Strings, Boolean</p></td>
<td align="left"><p>Numeric, Int, Character, Logical (and the pairlist)</p></td>
<td align="left"><p>Numbers, Char, Bool</p></td>
<td align="left"><p>Double precision is standard in all systems. Higher precision is only via libraries. Julia has a native 128 bit integer type.</p></td>
</tr>
<tr class="even">
<td align="left"><p>Native Data Structures</p></td>
<td align="left"><p>List, Tuple, Dict</p></td>
<td align="left"><p>List, Vector, Data Frame, Factor</p></td>
<td align="left"><p>Tuple, Dict, Set, Array, Vector, Matrix and more</p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>Object Oriented</p></td>
<td align="left"><p>Yes</p></td>
<td align="left"><p>Yes</p></td>
<td align="left"><p>Selective</p></td>
<td align="left"><p>R has a variety of Object Oriented implementations with different design and functionalities, they are denoted S3, S4, R5 and R6 respectively, Julia implements select OO aspects via the Struct composite type</p></td>
</tr>
<tr class="even">
<td align="left"><p>Code Structure</p></td>
<td align="left"><p>Based on Indentation</p></td>
<td align="left"><p>Free Style</p></td>
<td align="left"><p>Free Style</p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>Standard Libraries</p></td>
<td align="left"><p>Extensive</p></td>
<td align="left"><p>Built-in Functions</p></td>
<td align="left"><p>Base</p></td>
<td align="left"><p>Python has an extensive standard library as it covers a larger CS domain, In contrast R and Julia have a more extensive set of data science oriented features included by default</p></td>
</tr>
<tr class="even">
<td align="left"><p>Building Packages / Extensions</p></td>
<td align="left"><p><a href="https://docs.python.org/3/tutorial/modules.html">Modules</a>, <a href="https://docs.python.org/3/extending/building.html">Via bindings to C/C++</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/doc/manuals/R-exts.html#Creating-R-packages">Creating R packages</a></p></td>
<td align="left"><p><a href="https://julialang.github.io/Pkg.jl/v1/creating-packages/">Julia Packages</a></p></td>
<td align="left"><p>See below under HPC for more specific options</p></td>
</tr>
</tbody>
</table>

Development Environment
-----------------------

This section aims to answer the question: How can I develop and test code / applications written in Python, R or Julia?

<table>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<thead>
<tr class="header">
<th align="left"><p>Aspect</p></th>
<th align="left"><p>Python</p></th>
<th align="left"><p>R</p></th>
<th align="left"><p>Julia</p></th>
<th align="left"><p>Comment</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Open Source IDE's</p></td>
<td align="left"><p><a href="https://www.spyder-ide.org/">spyder</a>, <a href="https://netbeans.org/">netbeans</a>, <a href="https://www.eclipse.org/">eclipse</a>, <a href="https://code.visualstudio.com/">visual studio code</a></p></td>
<td align="left"><p><a href="https://www.rstudio.com/">R Studio</a>, <a href="https://docs.microsoft.com/en-us/visualstudio/rtvs/?view=vs-2017">RTVS</a></p></td>
<td align="left"><p><a href="https://junolab.org/">Juno</a></p></td>
<td align="left"><p>There are many other IDE's or advanced editors (Vim, Emacs etc.) that support programming languages via plugins. The degree of support varies (from syntax highlighting to supporting complete workflows within the IDE/editor)</p></td>
</tr>
<tr class="even">
<td align="left"><p>Commercial IDE's with Community Version</p></td>
<td align="left"><p>pycharm community / pro, komodo</p></td>
<td align="left"><p>R Studio</p></td>
<td align="left"><p>Intellij + Julia Plugin</p></td>
<td align="left"><p>Here we list closed source IDE's with free, or commercial versions</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Notebooks / Literate Programming</p></td>
<td align="left"><p><a href="https://jupyter.org/">Jupyter</a>, pweave</p></td>
<td align="left"><p>Jupyter, <a href="https://rmarkdown.rstudio.com/">R Markdown</a>, swave, knitr</p></td>
<td align="left"><p><a href="https://jupyter.org/">Jupyter</a>, <a href="https://github.com/JunoLab/Weave.jl">Weave.jl</a>, <a href="https://github.com/fredrikekre/Literate.jl">Literate.jl</a></p></td>
<td align="left"><p><em>Jupyter stands for Julia-Python-R Language!</em></p></td>
</tr>
<tr class="even">
<td align="left"><p>Debugger</p></td>
<td align="left"><p><a href="https://docs.python.org/3.7/library/pdb.html">pdb</a></p></td>
<td align="left"><p>various built-in functions (browser, traceback, debug)</p></td>
<td align="left"><p><a href="https://github.com/JuliaDebug/Debugger.jl">Debugger.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>Testing</p></td>
<td align="left"><p><a href="https://pypi.org/project/tox/">tox</a>, <a href="https://pytest.org/en/latest/">pytest</a>, <a href="https://docs.python.org/3/library/unittest.html">unittest</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/RUnit/index.html">runit</a>, <a href="https://cran.r-project.org/web/packages/testthat/index.html">testthat</a>, <a href="https://cran.r-project.org/web/packages/assertthat/index.html">assertthat</a></p></td>
<td align="left"><p>Base.test</p></td>
<td align="left"><p>(R testthat is for typical unit tests, R assertthat is to declare the pre and post conditions that code should satisfy)</p></td>
</tr>
<tr class="even">
<td align="left"><p><strong>Package Reviews</strong></p></td>
<td align="left"><p><a href="https://www.pythondatascience.org/Reproducibility.html">Reproducibility Task Views</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/views/ReproducibleResearch.html">Reproducible Research</a></p></td>
<td align="left"></td>
<td align="left"><p>Jupyter is available for all three systems</p></td>
</tr>
</tbody>
</table>

Files, Databases and Data Manipulation
--------------------------------------

This section aims to answer the following questions: What direct connectors to files stored on disk or data stored in databases are available for Python, R and Julia? Further, once we have connected to a data source, how can we fetch, store in memory and do preliminary work with the imported data?

<table>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<thead>
<tr class="header">
<th align="left"><p>Aspect</p></th>
<th align="left"><p>Python</p></th>
<th align="left"><p>R</p></th>
<th align="left"><p>Julia</p></th>
<th align="left"><p>Comment</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Loading Local Files</p></td>
<td align="left"><p>Builti-in, Pandas</p></td>
<td align="left"><p>Built-in</p></td>
<td align="left"><p>Built-in</p></td>
<td align="left"><p>General file input from local directories is built-in in all systems</p></td>
</tr>
<tr class="even">
<td align="left"><p>CSV Loading</p></td>
<td align="left"><p>Pandas</p></td>
<td align="left"><p>Built-in (read.csv), data.table, <a href="https://cran.r-project.org/web/packages/readr/index.html">readr</a></p></td>
<td align="left"><p><a href="https://github.com/JuliaData/CSV.jl">CSV.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>XLS/ODF Loading</p></td>
<td align="left"><p><a href="https://pypi.org/project/xlrd/">xlrd</a>, <a href="https://pypi.org/project/openpyxl/">openpyxl</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/XLConnect/index.html">XLConnect</a>, <a href="https://cran.r-project.org/web/packages/xlsx/index.html">xlsx</a></p></td>
<td align="left"><p><a href="https://github.com/sylvaticus/OdsIO.jl">OdsIO.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Hiearchical Data Formats (HDF)</p></td>
<td align="left"><p><a href="https://github.com/h5py/h5py">h5py</a>, pandas.read_hdf</p></td>
<td align="left"><p><a href="https://bioconductor.org/packages/release/bioc/html/rhdf5.html">rhdf5</a></p></td>
<td align="left"><p><a href="https://github.com/JuliaIO/HDF5.jl">HDF5.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>URL Requests</p></td>
<td align="left"><p><a href="https://pypi.org/project/requests/">requests</a>, <a href="https://pypi.org/project/pycurl/">PycURL</a></p></td>
<td align="left"><p>data.table, <a href="https://cran.r-project.org/web/packages/RCurl/index.html">rCurl</a></p></td>
<td align="left"><p><a href="https://github.com/JuliaWeb/HTTP.jl">HTTP.jl</a></p></td>
<td align="left"><p><em>The Julia package is still new and not tested in production systems</em></p></td>
</tr>
<tr class="even">
<td align="left"><p>Relational Database Connectors</p></td>
<td align="left"><p><a href="https://pypi.org/project/MySQL-python/">MySQLdb</a>, <a href="https://pypi.org/project/psycopg2/">psycopg2</a>, <a href="https://docs.python.org/3.7/library/sqlite3.html">sqlite3</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/RODBC/index.html">RODBC / RODBCExt</a>, <a href="https://cran.r-project.org/web/packages/RMySQL/index.html">RMySQL</a>, <a href="https://cran.r-project.org/web/packages/RPostgreSQL/index.html">RPostgresSQL</a>, <a href="https://cran.r-project.org/web/packages/RSQLite/index.html">RSQLite</a></p></td>
<td align="left"><p><a href="https://github.com/JuliaComputing/MySQL.jl">MySQL.jl</a>, <a href="https://github.com/JuliaDB/PostgreSQL.jl">PostgreSQL.jl</a>, <a href="https://github.com/JuliaDatabases/SQLite.jl">SQLite.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>Graph Databases Connectors</p></td>
<td align="left"><p><a href="https://pypi.org/project/neo4j/">neo4j</a>, <a href="https://pypi.org/project/pyArango/">pyArango</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/neo4r/index.html">neo4R</a></p></td>
<td align="left"><p><a href="https://github.com/glesica/Neo4j.jl">Neo4j.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Object Relational Mapping</p></td>
<td align="left"><p><a href="https://pypi.org/project/SQLAlchemy/">SQLAlchemy</a>, <a href="https://docs.djangoproject.com/en/2.2/topics/db/">Django ORM</a></p></td>
<td align="left"></td>
<td align="left"></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>General Data Wrangling</p></td>
<td align="left"><p><a href="https://pandas.pydata.org/">pandas</a></p></td>
<td align="left"><p>Built-in <a href="https://cran.r-project.org/web/packages/data.table/vignettes/datatable-intro.html">data.table</a>, (dplyr, tidyr, stringr, part of the <a href="https://www.tidyverse.org/packages/">tidyverse</a>)</p></td>
<td align="left"><p><a href="https://juliadata.github.io/DataFrames.jl/stable/">DataFrames.jl</a></p></td>
<td align="left"><p>The concept of a data frame has been a core aspect of R and pandas has emulated this in Python, DataFrame in Julia</p></td>
</tr>
<tr class="even">
<td align="left"><p>Missing Data</p></td>
<td align="left"><p>Pandas functionality, sklearn.impute</p></td>
<td align="left"><p>Amelia and many others</p></td>
<td align="left"><p><a href="https://github.com/invenia/Impute.jl">Impute.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>Advanced datetime handling</p></td>
<td align="left"><p><a href="https://pypi.org/project/python-dateutil/">dateutil</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/lubridate/">lubridate</a></p></td>
<td align="left"></td>
<td align="left"><p>These packages provide datetime specific extensions to built-in functionality</p></td>
</tr>
<tr class="even">
<td align="left"><p><strong>Package Reviews</strong></p></td>
<td align="left"><p><a href="https://www.pythondatascience.org/Databases.html">Databases Task Views</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/views/Databases.html">Databases</a>, <a href="https://cran.r-project.org/web/views/MissingData.html">Missing Data</a></p></td>
<td align="left"></td>
<td align="left"></td>
</tr>
</tbody>
</table>

General Purpose Mathematical Libraries
--------------------------------------

This section aims to answer the question: What building blocks are available for undertaking basic quantitative (numerical) work in Python, R and Julia respectively? NB: The division of what is *core mathematics* and what is a specialized domain is a bit arbitrary.

<table>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<thead>
<tr class="header">
<th align="left"><p>Aspect</p></th>
<th align="left"><p>Python</p></th>
<th align="left"><p>R</p></th>
<th align="left"><p>Julia</p></th>
<th align="left"><p>Comment</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>General Purpose vectors and n-dimensional arrays (as storage)</p></td>
<td align="left"><p><a href="https://www.numpy.org/">numpy</a></p></td>
<td align="left"><p>Built-in array</p></td>
<td align="left"></td>
<td align="left"><p>The R system comes with many basic array functionalities available built-in</p></td>
</tr>
<tr class="even">
<td align="left"><p>Numerical Linear Algebra (matrix operations)</p></td>
<td align="left"><p>numpy.linalg</p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/Matrix/index.html">Matrix</a>, <a href="https://cran.r-project.org/web/packages/RcppArmadillo/index.html">RcppArmadillo</a>, <a href="https://cran.r-project.org/web/packages/RcppEigen/index.html">RcppEigen</a></p></td>
<td align="left"><p>Built-in support (LinearAlgebra.Basic), StaticArrays, BandedMatrices, IterativeSolvers</p></td>
<td align="left"><p>For specialized operations (large / sparse matrices see below in HPC), eigenpy and pybind11 provide alternative means to use C++ numerical linear algebra in Python</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Mathematical (Special) Functions such as Gamma, Beta, Bessel</p></td>
<td align="left"><p><a href="https://www.scipy.org/">scipy</a></p></td>
<td align="left"><p>Built-in functions</p></td>
<td align="left"><p>SpecialFunctions.jl</p></td>
<td align="left"><p>| The R system comes with many basic functionalities available built-in</p></td>
</tr>
<tr class="even">
<td align="left"><p>Random Number Generation</p></td>
<td align="left"><p>Built-in, numpy.random</p></td>
<td align="left"><p>Built-in functions</p></td>
<td align="left"><p>Built-in (Random.Random)</p></td>
<td align="left"><p>This entry is about generic random numbers. More specialized applications mentioned below</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Mathematical Optimisation</p></td>
<td align="left"></td>
<td align="left"></td>
<td align="left"><p>JuMP</p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Symbolic Algebra</p></td>
<td align="left"><p><a href="https://www.sympy.org/en/index.html">sympy</a></p></td>
<td align="left"></td>
<td align="left"><p>Symata</p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>Curve Fitting</p></td>
<td align="left"><p>scipy.optimize, numpy.polyfit</p></td>
<td align="left"><p>Built-in</p></td>
<td align="left"><p>ApproxFun</p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p><strong>Package Reviews</strong></p></td>
<td align="left"><p><a href="https://www.pythondatascience.org/Mathematics.html">Mathematics Task Views</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/views/NumericalMathematics.html">Numerical Mathematics</a>, <a href="https://cran.r-project.org/web/views/Optimization.html">Optimization</a></p></td>
<td align="left"></td>
<td align="left"></td>
</tr>
</tbody>
</table>

Core Statistics Libraries
-------------------------

This section aims to answer the question: What libraries are available for undertaking standard statistical studies in Python, R or Julia? There is a large number of packages / modules with significant duplication / overlap, *especially for the R system*, hence only the major / indicative ones are considered.

<table>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<thead>
<tr class="header">
<th align="left"><p>Aspect</p></th>
<th align="left"><p>Python</p></th>
<th align="left"><p>R</p></th>
<th align="left"><p>Julia</p></th>
<th align="left"><p>Comment</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p><a href="Exploratory%20Data%20Analysis" title="wikilink">Exploratory Data Analysis</a> (descriptive statistics, moments, etc)</p></td>
<td align="left"><p>pandas.describe, <a href="https://github.com/pandas-profiling/pandas-profiling">pandas profiling</a>, scipy.stats, <a href="https://pypi.org/project/statsmodels/">statsmodels</a></p></td>
<td align="left"><p>Base R (stats), <a href="https://cran.r-project.org/web/packages/car/index.html">car</a>, <a href="https://cran.r-project.org/web/packages/caret/index.html">caret</a>, dplyr</p></td>
<td align="left"><p>describe(DataFrame)</p></td>
<td align="left"><p>EDA is quite broad and loosely defined. Here we take a fairly narrow view that remains as much as possible non-parametric and model-agnostic</p></td>
</tr>
<tr class="even">
<td align="left"><p>Correlation</p></td>
<td align="left"><p>pandas.corr, numpy.corrcoef</p></td>
<td align="left"><p>Built-in (cor)</p></td>
<td align="left"><p>Built-in (cor)</p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>ANOVA</p></td>
<td align="left"><p>scipy.stats, statsmodels</p></td>
<td align="left"><p>Built-in (aov, anova), car, caret</p></td>
<td align="left"><p><a href="https://github.com/marcpabst/ANOVA.jl">ANOVA.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Linear Regression Analysis</p></td>
<td align="left"><p><a href="https://scikit-learn.org/stable/index.html">scikit-learn</a>, statsmodels</p></td>
<td align="left"><p>Built-in</p></td>
<td align="left"><p><a href="https://github.com/lindahua/Regression.jl">Regression.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>Generalized Linear Regression</p></td>
<td align="left"><p>scikit-learn, statsmodels</p></td>
<td align="left"><p>Built-in <a href="https://cran.r-project.org/web/packages/glmnet/index.html">glmnet</a></p></td>
<td align="left"><p>Regression.jl</p></td>
<td align="left"><p>This category includes logistic regression (which is available in many R packages), multinomial regression etc.</p></td>
</tr>
<tr class="even">
<td align="left"><p>Survival Analysis</p></td>
<td align="left"><p><a href="https://pypi.org/project/lifelines/">lifelines</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/views/Survival.html">survival</a></p></td>
<td align="left"><p><a href="https://github.com/JuliaStats/Survival.jl">Survival.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>Gaussian Processes</p></td>
<td align="left"><p><a href="https://github.com/SheffieldML/GPy">GPy</a></p></td>
<td align="left"><p>GauPro, GPfit, kergp, mlegp</p></td>
<td align="left"><p>GaussianProcesses.jl</p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p><strong>Package Reviews</strong></p></td>
<td align="left"><p><a href="https://www.pythondatascience.org/Statistics.html">Statistics Task Views</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/views/Distributions.html">Probability Distributions</a>, <a href="https://cran.r-project.org/web/views/Multivariate.html">Multivariate Statistics</a>, <a href="https://cran.r-project.org/web/views/ExtremeValue.html">Extreme Value Analysis</a>, <a href="https://cran.r-project.org/web/views/Robust.html">Robust Statistical Methods</a>, <a href="https://cran.r-project.org/web/views/Survival.html">Survival Analysis</a></p></td>
<td align="left"></td>
<td align="left"></td>
</tr>
</tbody>
</table>

Econometrics / Timeseries Libraries
-----------------------------------

This section aims to answer the question: What libraries are available for undertaking econometric / timeseries studies in Python, R or Julia?

<table>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<thead>
<tr class="header">
<th align="left"><p>Aspect</p></th>
<th align="left"><p>Python</p></th>
<th align="left"><p>R</p></th>
<th align="left"><p>Julia</p></th>
<th align="left"><p>Comment</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Basic Econometric Analysis (stationarity, trends, seasonality)</p></td>
<td align="left"><p>statsmodels.tsa</p></td>
<td align="left"><p>Built-in (ts)</p></td>
<td align="left"><p><a href="https://github.com/JuliaStats/TimeSeries.jl">TimeSeries.jl</a>, <a href="https://github.com/JuliaFinMetriX/Econometrics.jl">Econometrics.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>ARMA Processes / Univariate Models</p></td>
<td align="left"><p>statsmodels.tsa, <a href="https://www.alkaline-ml.com/pmdarima/index.html">pmdarima</a></p></td>
<td align="left"><p>auto, <a href="https://cran.r-project.org/web/packages/forecast/index.html">forecast</a>, <a href="https://cran.r-project.org/web/packages/tseries/index.html">tseries</a></p></td>
<td align="left"><p><a href="https://github.com/s-broda/ARCHModels.jl">ARCHModels.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>Heteroskedastic (GARCH) processes</p></td>
<td align="left"><p>statsmodels, <a href="https://pypi.org/project/arch/">arch</a></p></td>
<td align="left"><p>tseries, <a href="https://cran.r-project.org/web/packages/zoo/index.html">zoo</a>, vars</p></td>
<td align="left"><p>ARCHModels.jl</p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Vector Auto Regressions (VAR)</p></td>
<td align="left"><p>statsmodels.tsa</p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/MTS/index.html">mts</a>, <a href="https://cran.r-project.org/web/packages/vars/index.html">vars</a></p></td>
<td align="left"><p><a href="https://github.com/lucabrugnolini/VectorAutoregressions.jl">VectorAutoregressions.jl</a> (WIP)</p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>General Timeseries</p></td>
<td align="left"><p><a href="https://pypi.org/project/pyflux/">pflux</a>, <a href="https://facebook.github.io/prophet/docs/quick_start.html">prophet</a></p></td>
<td align="left"><p>prophet (R API)</p></td>
<td align="left"><p>TimeSeries.jl</p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Frequency Domain Analysis</p></td>
<td align="left"><p>numpy.fft</p></td>
<td align="left"><p>Built-in (spectrum)</p></td>
<td align="left"></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p><strong>Package Reviews</strong></p></td>
<td align="left"><p><a href="https://www.pythondatascience.org/Econometrics.html">Econometrics Task Views</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/views/Econometrics.html">Econometrics</a>, <a href="https://cran.r-project.org/web/views/TimeSeries.html">Time Series Analysis</a></p></td>
<td align="left"></td>
<td align="left"></td>
</tr>
</tbody>
</table>

Machine Learning Libraries
--------------------------

This section aims to answer the question: What libraries are available for machine learning projects in Python, R or Julia? The term machine learning is not too specific so we use this category to group various advanced / specialized libraries that are relevant for data science (but not e.g. computer vision and other specialized ML applications). NB: Machine learning algorithms are typically compute intensive and are thus implemented in system languages with eventual binding and API provided to Python or R environments

<table>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<thead>
<tr class="header">
<th align="left"><p>Aspect</p></th>
<th align="left"><p>Python</p></th>
<th align="left"><p>R</p></th>
<th align="left"><p>Julia</p></th>
<th align="left"><p>Comment</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Network Analysis</p></td>
<td align="left"><p><a href="https://pypi.org/project/networkx/">networkx</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/igraph/index.html">igraph</a>, <a href="https://cran.r-project.org/web/packages/sna/index.html">sna</a></p></td>
<td align="left"><p><a href="https://github.com/JuliaGraphs/LightGraphs.jl">LightGraphs.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Cluster Analysis (Unsupervised Learning)</p></td>
<td align="left"><p>scikit-learn</p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/cluster/index.html">cluster</a></p></td>
<td align="left"><p><a href="https://github.com/JuliaStats/Clustering.jl">Clustering.jl</a></p></td>
<td align="left"><p>K-means and other clustering algorithms</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Random Forests</p></td>
<td align="left"><p>scikit-learn</p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/randomForest/index.html">randomForest</a>, <a href="https://cran.r-project.org/web/packages/ranger/index.html">ranger</a></p></td>
<td align="left"><p><a href="https://github.com/bensadeghi/DecisionTree.jl">DecisionTree.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Gradient Boosting</p></td>
<td align="left"><p>scikit-learn</p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/xgboost/index.html">XGBoost Interface</a></p></td>
<td align="left"><p><a href="https://github.com/dmlc/XGBoost.jl">XGBoost.jl Interface</a></p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>Probabilistic Graphical Models</p></td>
<td align="left"><p><a href="https://pgmpy.org/">pgmpy</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/bnlearn/index.html">bnlearn</a>, <a href="https://cran.r-project.org/web/packages/gRain/index.html">gRain</a></p></td>
<td align="left"><p><a href="https://github.com/JuliaStats/PGM.jl">PGM.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Neural Networks</p></td>
<td align="left"><p><a href="https://www.tensorflow.org/">tensorflow</a>, <a href="https://pytorch.org/">pytorch</a>, <a href="https://keras.io/">keras</a>, <a href="https://mxnet.incubator.apache.org/api/python/index.html">Interface to MXNet</a></p></td>
<td align="left"><p><a href="https://keras.io/">Interface to h2o</a>, <a href="https://github.com/apache/incubator-mxnet/tree/master/R-package">Interface to MXNet</a>, <a href="https://cran.r-project.org/web/packages/kerasR/vignettes/introduction.html">Interface to keras</a></p></td>
<td align="left"><p>Flux, MLJ, Knet</p></td>
<td align="left"><p>R studio offers an <a href="https://tensorflow.rstudio.com/">interface to tensorflow</a></p></td>
</tr>
<tr class="odd">
<td align="left"><p><strong>Package Review</strong></p></td>
<td align="left"><p><a href="https://www.pythondatascience.org/MachineLearning.html">Machine Learning Task Views</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/views/Bayesian.html">Bayesian Inference</a>, <a href="https://cran.r-project.org/web/views/Cluster.html">Cluster Analysis &amp; Finite Mixture Models</a>, <a href="https://cran.r-project.org/web/views/MachineLearning.html">Machine Learning</a>, <a href="https://cran.r-project.org/web/views/gR.html">Graphical Models</a></p></td>
<td align="left"></td>
<td align="left"></td>
</tr>
</tbody>
</table>

GeoSpatial Libraries
--------------------

This section aims to answer the question: What libraries are available for working with GIS / geospatial data in Python, R or Julia? The geospatial package space is particularly fragmented, the selection focuses on some key *anchor* concepts.

<table>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<thead>
<tr class="header">
<th align="left"><p>Aspect</p></th>
<th align="left"><p>Python</p></th>
<th align="left"><p>R</p></th>
<th align="left"><p>Julia</p></th>
<th align="left"><p>Comment</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Geo Data Structures</p></td>
<td align="left"><p>GeoPandas.GeoSeries, GeoPandas.GeoDataFrame</p></td>
<td align="left"><p>raster, sp, sf, stars</p></td>
<td align="left"></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>GDAL</p></td>
<td align="left"><p><a href="https://gdal.org/">gdal</a></p></td>
<td align="left"><p>rgdal</p></td>
<td align="left"><p><a href="https://github.com/JuliaGeo/GDAL.jl">GDAL.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>GeoJSON</p></td>
<td align="left"><p><a href="https://pypi.org/project/geojson/">geojson</a></p></td>
<td align="left"><p>geojson, rgdal</p></td>
<td align="left"><p>GeoJSON</p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>PostGIS</p></td>
<td align="left"><p><a href="https://pypi.org/project/geojson/">geojson</a></p></td>
<td align="left"><p>rpostgis</p></td>
<td align="left"><p>GeoJSON</p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>GeoMaping</p></td>
<td align="left"><p>CartoPy, Descartes</p></td>
<td align="left"><p>gmt</p></td>
<td align="left"><p>GMT</p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>OpenStreetMap</p></td>
<td align="left"><p><a href="https://pypi.org/project/openstreetmap/">openstreetmap</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/OpenStreetMap/index.html">OpenStreetMap</a></p></td>
<td align="left"><p><a href="https://github.com/tedsteiner/OpenStreetMap.jl">OpenStreetMap.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>Spatial Statistics</p></td>
<td align="left"><p>pysal</p></td>
<td align="left"><p>gstat, geoR, geoRglm</p></td>
<td align="left"></td>
<td align="left"><p>R has a large number of specialized spatial statistics packages (see Task Views)</p></td>
</tr>
<tr class="even">
<td align="left"><p>Spatial Econometrics</p></td>
<td align="left"><p><a href="https://pysal.readthedocs.io/en/v1.11.0/users/tutorials/econometrics.html">pysal.spreg</a></p></td>
<td align="left"></td>
<td align="left"></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p><strong>Package Review</strong></p></td>
<td align="left"><p><a href="https://www.pythondatascience.org/Geospatial.html">Geospatial Task Views</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/views/Spatial.html">Spatial Data</a>, <a href="https://cran.r-project.org/web/views/SpatioTemporal.html">Handling and Analyzing Spatio-Temporal Data</a></p></td>
<td align="left"></td>
<td align="left"></td>
</tr>
</tbody>
</table>

Visualization
-------------

This section aims to answer the question: What functionality is available to produce *data driven* visualization in Python, R or Julia?

<table>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<thead>
<tr class="header">
<th align="left"><p>Aspect</p></th>
<th align="left"><p>Python</p></th>
<th align="left"><p>R</p></th>
<th align="left"><p>Julia</p></th>
<th align="left"><p>Comment</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Low level API's</p></td>
<td align="left"><p><a href="https://matplotlib.org/">matplotlib</a></p></td>
<td align="left"><p><a href="https://bookdown.org/rdpeng/RProgDA/the-grid-package.html">grid</a>, gridExtra</p></td>
<td align="left"><p><a href="https://github.com/JuliaPlots/Plots.jl">Plots.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Graph packages</p></td>
<td align="left"><p><a href="https://pypi.org/project/seaborn/">seaborn</a>, <a href="https://pypi.org/project/plotly/">plotly</a>, <a href="https://pypi.org/project/bokeh/">bokeh</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/ggplot2/index.html">ggplot2</a></p></td>
<td align="left"><p><a href="https://github.com/GiovineItalia/Gadfly.jl">Gadfly.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>Declarative Visualizations</p></td>
<td align="left"><p><a href="https://altair-viz.github.io/">Altair</a></p></td>
<td align="left"></td>
<td align="left"><p>Vega.jl</p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>XKCD style plots :-)</p></td>
<td align="left"><p><a href="https://matplotlib.org/xkcd/examples/showcase/xkcd.html">Available!</a></p></td>
<td align="left"><p><a href="http://xkcd.r-forge.r-project.org/">Available!</a></p></td>
<td align="left"></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p><strong>Package Review</strong></p></td>
<td align="left"><p><a href="https://www.pythondatascience.org/Visualization.html">Visualization Task Views</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/views/Graphics.html">Graphic Displays &amp; Visualization</a></p></td>
<td align="left"></td>
<td align="left"></td>
</tr>
</tbody>
</table>

Web, Desktop and Mobile Deployment
----------------------------------

This section aims to answer the question: What tools does each language ecosystem provide for the *deployment of data based applications*, whether this is via the web, desktop or mobile apps.

<table>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<thead>
<tr class="header">
<th align="left"><p>Aspect</p></th>
<th align="left"><p>Python</p></th>
<th align="left"><p>R</p></th>
<th align="left"><p>Julia</p></th>
<th align="left"><p>Comment</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Native Webservers</p></td>
<td align="left"><p><a href="https://pypi.org/project/tornado/">Tornado</a>, <a href="https://pypi.org/project/gunicorn/">Gunicorn</a>, <a href="https://pypi.org/project/CherryPy/">CherryPy</a>, <a href="https://pypi.org/project/Twisted/">Twisted</a></p></td>
<td align="left"><p><a href="https://www.opencpu.org/">OpenCPU</a>, <a href="https://cran.r-project.org/web/packages/plumber/index.html">plumber</a></p></td>
<td align="left"><p><a href="https://github.com/JuliaWeb/HTTP.jl">HTTP.jl</a></p></td>
<td align="left"><p>As a general remark these native servers are not exposed directly in production but are fronted by e.g. apache httpd and nginx servers</p></td>
</tr>
<tr class="even">
<td align="left"><p>Classic Web Frameworks</p></td>
<td align="left"><p><a href="https://pypi.org/project/Flask/">Flask</a>, <a href="https://pypi.org/project/pyramid/">Pyramid</a>, <a href="https://pypi.org/project/Django/">Django</a></p></td>
<td align="left"><p><a href="https://www.rstudio.com/products/shiny/">R Shiny</a>, <a href="http://rapache.net/">rApache</a></p></td>
<td align="left"><p><a href="https://github.com/genieframework/Genie.jl">Genie.jl</a></p></td>
<td align="left"><p>Web frameworks typically used behind a production web server (<a href="https://httpd.apache.org/">Apache</a>, <a href="https://nginx.org/en/">Nginx</a> etc.)</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Web Formats</p></td>
<td align="left"><p>xml, json (built-in)</p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/XML/index.html">XML</a>, <a href="https://cran.r-project.org/web/packages/rjson/index.html">rjson</a>, <a href="https://cran.r-project.org/web/packages/jsonlite/index.html">jsonlite</a></p></td>
<td align="left"><p><a href="https://github.com/JuliaIO/JSON.jl">JSON.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Web Sockets</p></td>
<td align="left"><p><a href="https://pypi.org/project/websockets/">websockets</a></p></td>
<td align="left"></td>
<td align="left"><p><a href="https://github.com/JuliaWeb/WebSockets.jl">WebSockets.jl</a></p></td>
<td align="left"><p>WebSocket connection allows full-duplex communication between a client and server so that either side can push data to the other through an established connection</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Client Side (Browser)</p></td>
<td align="left"><p><a href="https://brython.info/">Brython</a>, <a href="https://docs.rs/rustpython-vm/0.1.0/rustpython_vm/">RustPython</a>, <a href="https://pyodide.readthedocs.io/en/latest/">Pyodide</a></p></td>
<td align="left"></td>
<td align="left"></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Mobile Apps</p></td>
<td align="left"><p><a href="https://kivy.org/#home">Kivy</a>, <a href="https://pypi.org/project/beeware/">Beeware</a></p></td>
<td align="left"></td>
<td align="left"></td>
<td align="left"><p>Both kivy and beeware allow cross-platform app development.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><strong>Package Review</strong></p></td>
<td align="left"><p><a href="https://www.pythondatascience.org/Web.html">Web Task Views</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/views/ModelDeployment.html">Model Deployment</a>, <a href="https://cran.r-project.org/web/views/WebTechnologies.html">Web Technologies</a></p></td>
<td align="left"></td>
<td align="left"></td>
</tr>
</tbody>
</table>

Semantic Web / Semantic Data
----------------------------

This section aims to answer the question: What tools and libraries are available for working with semantic data (RDF, OWL, JSON-LD etc) and other relevant domain specific metadata schemas?

<table>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<thead>
<tr class="header">
<th align="left"><p>Aspect</p></th>
<th align="left"><p>Python</p></th>
<th align="left"><p>R</p></th>
<th align="left"><p>Julia</p></th>
<th align="left"><p>Comment</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>RDF Format</p></td>
<td align="left"><p>rdflib</p></td>
<td align="left"><p>rrdf</p></td>
<td align="left"></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>JSON-LD Format</p></td>
<td align="left"><p>rdflib.jsonld</p></td>
<td align="left"></td>
<td align="left"></td>
<td align="left"><p>JSON-LD is an alternative web-friendly serialization format for RDF</p></td>
</tr>
<tr class="odd">
<td align="left"><p>OWL Ontologies</p></td>
<td align="left"><p>ontospy, owlready2</p></td>
<td align="left"></td>
<td align="left"></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Querying RDF (SPARQL)</p></td>
<td align="left"><p>rdflib</p></td>
<td align="left"><p>Rredland</p></td>
<td align="left"></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>Serving RDF (SPARQL)</p></td>
<td align="left"><p>rdflib</p></td>
<td align="left"></td>
<td align="left"></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>SDMX Format</p></td>
<td align="left"><p><a href="https://pandasdmx.readthedocs.io/en/stable/">pandasdmx</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/rsdmx/index.html">rsdmx</a></p></td>
<td align="left"></td>
<td align="left"><p>SDMX is the <a href="https://sdmx.org/">statistical data and metadata exchange</a> format</p></td>
</tr>
<tr class="odd">
<td align="left"><p><strong>Package Review</strong></p></td>
<td align="left"><p><a href="https://www.pythondatascience.org/SemanticData.html">Semantic Data Task View</a></p></td>
<td align="left"></td>
<td align="left"></td>
<td align="left"></td>
</tr>
</tbody>
</table>

High Performance Computing
--------------------------

For our purposes high performance computing (HPC) is any use case that requires more than a single CPU (and its own RAM or disk). This section aims to answer the question: what are my options if I have performance bottlenecks in terms of CPU, memory or disk, hence covering topics such as concurrency or GPU computing. NB: Julia aims to address performance issues through compilation and other design choices

<table>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<thead>
<tr class="header">
<th align="left"><p>Aspect</p></th>
<th align="left"><p>Python</p></th>
<th align="left"><p>R</p></th>
<th align="left"><p>Julia</p></th>
<th align="left"><p>Comment</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Bindings to C/C++</p></td>
<td align="left"><p><a href="https://cython.org/">Cython</a>, <a href="https://pypi.org/project/pybind11/">pybind11</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/Rcpp/index.html">Rcpp</a></p></td>
<td align="left"><p><a href="https://github.com/JuliaInterop/Cxx.jl">Cxx.jl</a></p></td>
<td align="left"><p>Native Python, R are slow compared to lower level / compiled languages. A common approach to make full use of existing CPU is to extend the language via bindings to a faster language. Bindings might also be useful to re-use existing libraries</p></td>
</tr>
<tr class="even">
<td align="left"><p>Bindings to Java</p></td>
<td align="left"><p><a href="https://pypi.org/project/py4j/">py4j</a>, <a href="https://pypi.org/project/pyo3-pack/">pyO3</a></p></td>
<td align="left"><p>renjin</p></td>
<td align="left"><p><a href="https://github.com/JuliaInterop/JavaCall.jl">JavaCall.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>Bindings to other performing languages (Rust etc)</p></td>
<td align="left"><p><a href="https://pypi.org/project/pyo3-pack/">pyO3</a></p></td>
<td align="left"></td>
<td align="left"></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Coroutines</p></td>
<td align="left"><p>Built-in (async/await, since Python 3.5)</p></td>
<td align="left"></td>
<td align="left"><p>Built-in (Tasks/Channels)</p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>Multi-threading</p></td>
<td align="left"><p>Built-in (thread)</p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/foreach/index.html">foreach</a></p></td>
<td align="left"><p>Built-in (Base.Threads) (Experimental)</p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Multi-core</p></td>
<td align="left"><p><a href="https://pypi.org/project/multiprocessing/">multiprocessing</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/doParallel/index.html">doParallel</a>, <a href="https://cran.r-project.org/web/packages/future/index.html">future</a></p></td>
<td align="left"><p>Built-in (Distributed)</p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>Spark interface</p></td>
<td align="left"><p><a href="https://pypi.org/project/pyspark/">pySpark</a></p></td>
<td align="left"><p>SparkR, <a href="https://cran.r-project.org/web/packages/sparklyr/index.html">sparklyr</a></p></td>
<td align="left"><p><a href="https://github.com/dfdx/Spark.jl">Spark.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>GPU Computing</p></td>
<td align="left"><p><a href="https://pypi.org/project/pycuda/">pyCUDA</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/gpuR/index.html">gpuR</a></p></td>
<td align="left"><p><a href="https://github.com/JuliaGPU/CUDAnative.jl">CUDAnative.jl</a></p></td>
<td align="left"><p>GPU interfaces are offered also via some ML packages (e.g pytorch, tensorflow, MXnet.jl)</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Distributed Data</p></td>
<td align="left"><p><a href="https://pypi.org/project/dask/">dask</a></p></td>
<td align="left"><p><a href="https://github.com/tidyverse/multidplyr">multidplyr</a></p></td>
<td align="left"><p><a href="https://github.com/JuliaComputing/JuliaDB.jl">JuliaDB.jl</a></p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p><strong>Package Review</strong></p></td>
<td align="left"><p><a href="https://www.pythondatascience.org/HPC.html">HPC Task Views</a></p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/views/HighPerformanceComputing.html">High-Performance and Parallel Computing</a></p></td>
<td align="left"></td>
<td align="left"></td>
</tr>
</tbody>
</table>

Using R, Python and Julia together
----------------------------------

The section aims to answer the question: How can I use R from Python, Python from Julia, Julia from R and *vice versa* :-). The first rows of this table have the From/To Format (From X Call Y) for native integration between the three systems, where "Native" means that the integration is done using language bindings within the respective interpreters / REPL (not explicitly using the operating system or a server API)

<table>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<thead>
<tr class="header">
<th align="left"><p>Aspect</p></th>
<th align="left"><p>Call Python</p></th>
<th align="left"><p>Call R</p></th>
<th align="left"><p>Call Julia</p></th>
<th align="left"><p>Comment</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>From Python</p></td>
<td align="left"></td>
<td align="left"><p><a href="https://pypi.org/project/rpy2/">rpy2</a></p></td>
<td align="left"><p><a href="https://github.com/JuliaPy/pyjulia">pyjulia</a></p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>From R</p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/PythonInR/index.html">PythonInR</a>, <a href="https://cran.r-project.org/web/packages/rPython/index.html">rPython</a></p></td>
<td align="left"></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/XRJulia/index.html">XRJulia</a></p></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>From Julia</p></td>
<td align="left"><p><a href="https://github.com/JuliaPy/PyCall.jl">PyCall.jl</a></p></td>
<td align="left"><p><a href="https://github.com/JuliaInterop/RCall.jl">RCall.jl</a></p></td>
<td align="left"></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Python/R Cross-Development and Integration</p></td>
<td align="left"><p><a href="https://github.com/holgerbrandl/r4intellij">r4intellij</a>, rpy2</p></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/reticulate/index.html">reticulate</a></p></td>
<td align="left"></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><p>Via Server API's</p></td>
<td align="left"></td>
<td align="left"><p><a href="https://cran.r-project.org/web/packages/Rserve/index.html">Rserve</a></p></td>
<td align="left"></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Via OS / Shell Scripts</p></td>
<td align="left"><p>Built-in (subprocess)</p></td>
<td align="left"><p>Built-in (system2)</p></td>
<td align="left"><p>Built-in (Base.run)</p></td>
<td align="left"></td>
</tr>
</tbody>
</table>