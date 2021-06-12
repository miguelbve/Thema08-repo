Jurriën de Jong and Miguel Botter van Elburg
Sat 12 Jun 2021
Version 1





Name
====
Cardiac drug efficacy model




Description
===========
Cardiac drug analysis is a powerful approach for analyzing mathematical models comprised of a few ordinary differential equations (ODEs). reproduced_research.Rmd is an professional Rmd-script allowing one to easily reproduce such models by numerical integration, finding and following steady states, and fitting to data. Thema08-repo is easy to use because it includes just a few files, which can be ruled by the main file reproduced_research.Rmd

reproduced_research.Rmd is a r programming language based program whose you can execute via the Rstudio GUI, specially via the knitr button. It is used for generating the research report in pdf format, whose aims to provide a better understanding of the drug concentration over time in different tissue types of the heart. The fabricated pdf files has been rendered for our final project this year for the Hanze Hogeschool Groningen, this all happened under supervision of the scientific research programmer and university lecturer Fenna Feenstra.

For reviewing our project repository, visit 'https://github.com/miguelbve/Thema08-repo.git'




Requirements
============
The following software/packages are required, to get most out of the reproduced_research.Rmd and all the additional files

"git"
"stats"     
"graphics"  
"grDevices" 
"utils"     
"datasets"  
"methods"   
"base"
"A version of R 4.X"
"RStudio Desktop app or RStudio 1.4 Server" [To reproduce this research, this software is required, altough our software can be executed via the command line interface, or R Console, we've used the RStudio for producing our end product]




Installation
============
When you read this at the github repisotory, the first thing you need to do, if you want to get the pdf rendered locally, is to clone the repository. After each explanation, there is an example of what your action should look like. In this manner you will be guided to use our software properly and reproduce as good as possible.



--STEP 1 -- execute the following command in your zsh or bash implemented terminal.
	~$ git clone https://github.com/miguelbve/Thema08-repo.git
	
--STEP 2 -- change your directory to the final research directory, within that directory the reproduced_research.Rmd can be found. If you made it this far you're installation is ready!
	~$ cd Thema08-repo/research/
Note: It is recommended (not required) to go to the above mentioned directory via the RStudio Desktop application or RStudio Server, this makes life much easier for further steps. Now you're able to use the software. Please go to the next 'Usage' section and follow briefly the instructions involved the usage of the reproduced_research.Rmd program.




Usage
=====
To use our software, there are some commands necessary to generate the end result (the rendered pdf file). To obtain the output pdf file result make sure you've executed the program file thema02_opdracht.py. You can do this by following the instructions below. Again, after each explanation, there is a example of what your action should look like. In this manner you will be guided to use our software properly and reproduce as good as possible.



--STEP 1-- Step 1. Execute the main program called reproduced_research.Rmd by using the knit button in the RStudio or RStudio Server. 
Note: To render the main program properly, it is important to obtain of the required packages mentioned earlier. Since this file tries to load additional R packages which are essential for the models used in the research.


There will be displayed some information while knitting, make sure you don't obtain any errors, if you do, go back and redo all steps, until you don't receive any errors. If you get stuck at this step without any pdf output file. You are more than welcome to contact one of the contributers, you can find information about them in the end of this documentation in the Authors and acknowledgment section 


processing file: reproduced_research.Rmd
  |.........                                                             |  12%
   inline R code fragments

  |..................                                                    |  25%
label: setup (with options) 
List of 1
 $ include: logi FALSE

  |..........................                                            |  38%
  ordinary text without R code

  |...................................                                   |  50%
label: research_code_echo (with options) 
List of 1
 $ echo: logi FALSE

  |............................................                          |  62%
  ordinary text without R code

  |....................................................                  |  75%
label: unnamed-chunk-1 (with options) 
List of 1
 $ echo: logi FALSE

  |.............................................................         |  88%
  ordinary text without R code

  |......................................................................| 100%
label: research_code

output file: reproduced_research.knit.md

/usr/lib/rstudio-server/bin/pandoc/pandoc +RTS -K512m -RTS reproduced_research.utf8.md --to latex --from markdown+autolink_bare_uris+tex_math_single_backslash --output reproduced_research.tex --lua-filter /homes/lmabottervanelburg/R/x86_64-pc-linux-gnu-library/4.0/rmarkdown/rmarkdown/lua/pagebreak.lua --lua-filter /homes/lmabottervanelburg/R/x86_64-pc-linux-gnu-library/4.0/rmarkdown/rmarkdown/lua/latex-div.lua --self-contained --number-sections --highlight-style tango --pdf-engine pdflatex --variable graphics --include-in-header /tmp/RtmpYD6e1G/rmarkdown-str3b36ea5e254e91.html --variable 'geometry:margin=1in' --citeproc 

Output created: reproduced_research.pdf


- Don't worry about overwriting the earlier included reproduced_research.Rmd file, this means that the main file just can run the additional package dependencies!


The most important notification in your R Markdown console should be the following
output file: reproduced_research.knit.md

/usr/lib/rstudio-server/bin/pandoc/pandoc +RTS -K512m -RTS reproduced_research.utf8.md --to latex --from markdown+autolink_bare_uris+tex_math_single_backslash --output reproduced_research.tex --lua-filter /homes/lmabottervanelburg/R/x86_64-pc-linux-gnu-library/4.0/rmarkdown/rmarkdown/lua/pagebreak.lua --lua-filter /homes/lmabottervanelburg/R/x86_64-pc-linux-gnu-library/4.0/rmarkdown/rmarkdown/lua/latex-div.lua --self-contained --number-sections --highlight-style tango --pdf-engine pdflatex --variable graphics --include-in-header /tmp/RtmpYD6e1G/rmarkdown-str3b36ea5e254e91.html --variable 'geometry:margin=1in' --citeproc 

Output created: reproduced_research.pdf"

Then the file research is converted to a file in pdf format and you should be ready to gaze the dedicated report.




Support
=======
for questions about our project 'thema02_opdracht.py', you're able to contact us via mail.
	*Jurriën ju.de.jong@st.hanze.nl	
	*Miguel		l.m.a.botter.van.elburg@st.hanze.nl




Authors and acknowledgment
==========================
We want to thank our lecturer, Fenna Feenstra, she contributed to our report and the final project. For instance, she gave us important feedback and she trains
us to decompose problems in a more scientific way. That will be quite helpful for making better research projects like these in the future.
At last but not least, we want to thank Michiel Noback. He provided us some extra tips for plotting ggplot, which was a huge resource for development for our plotted graphs.