# __Intern_journal__  :kenya: 🔬:

## __Hello!__ 👋:

__Greetings and welcome__  thank you for checking out my page. I am an aspiring bioinformaticians with a background in biochemistry. during my undergraduate course, I found myself drawn to the multidisciplinary of the field as I undertook my first attachment. since then, I have taken steps to further my knowledge in the trade here are some of my credentials 
[link][1] 

[1]:https://credentials.edx.org/records/programs/shared/bd4759839c9c4d0c9e6eeb8a4c472587/ 
The need for computational scientist globally is rising, and with it I dream to rise and distinguish myself as a professional in the field. 

Here I will document my journey through ICIPE cohort 6 internship

## Vision

My vision for this internship is to jump start my career as a bioinformatician and network with others in the field. Additionally I would also like to be able to submit a useful package in R to the CRAN that can be used to analyze and visualize proteomic and/or genomic data, carry out MSA  and generate a workflow from this code that I can be reusing. to this end I will need to:

1. Understand additional tools that are used by bioinformaticians
2. Utilize the trainers wealth of information and time 
3. Tap into the strengths of my teammates and solve problems that I've encountered in R studio.
4. reproduce a similar project 
5. Share any information I have gained hitherto.

## __Mission__

My main mission is to contribute to the scientific community by using the skills I'll learn from this internship to unlock different secrets of the molecular world, secrets that could potentially cure disease and improve the quality of life . Using programming tools I would like to help generate reusable scripts to visualize data that others could use as a standard in various research projects.

## Day one(understanding git and GitHub)

### forking and cloning
forking a repository is basically making a copy of an already existing project that you can work on separately. while cloning is allows you to have a copy of the file on your PC.

if the changes you've made to the project are useful then you can make a pull request for the changes to be added. here is a link to my first attempt [link][1]

[1]:https://github.com/Mattcreates25/MyFirstFork

### Why fork  

1. Use someone's project as a starting point for yours
2. Make proposal edits to someones work.

### markdown

markdown is a way to format text  on GitHub

here is an example of a function from one of my projects wrapped in back ticks
```r
slidingwindowGCplot= function(windowsize, inputseq)
{GCwindow= seq(1,length(inputseq)- windowsize, by= windowsize)
  #find the length of the GC window
    n= length(GCwindow)
        #make an empty vector with the same length
          chunks=numeric(n)
          for (i in 1:n) {
            chunk=inputseq[GCwindow[i]:(GCwindow[i]+ windowsize-1)]
            chunkGC= GC(chunk)
            print(chunkGC)
            chunks[i]= chunkGC
          }
          #generate plots for the sliding window
          plot(GCwindow, chunks, type= "b", 
               xlab = "nucleotide start position", 
               ylab = "GC content", 
               main=paste("GC plot with windowsize", windowsize))
          ##the second part of the main part is the variable. in this case windowsize
          
          }
 ```

using markdown i'm able to wrap my code and specify the language that I used for this code.

## __DAY two(open science)__

refresher on issue tracking on GitHub
open science and data management in bioinformatics
what is open science.. contribute, collaborate, redistribute and reproduce, transparent, accessible , available and free
why open science fostering a scientific ecosystem, benefits of open access, increased quality of the research , increase opportunities, faster transfer of knowledge, foster innovation, improves productivity and research output, improves willingness in participants
taxonomy open science: open access, open data , open reproducible
open access journal: F1000 research, <AAs open access journal , wellcome open research , e life(avoid predatory journals)
tools: >R markdown, jupyter hub,zenodo, galaxy project, nextflow, docker
data management: FAIR(findable, accessible, inter-operable and reusable
data management plan: types of data, standard, format, metadata, provisions for archiving  and preservation, access policies
organizing your sequencing project: data tidiness, data storage 





# __ROAD MAP__ :checkered_flag:

## __milestone 1__ :pushpin:
getting to understand git and GitHub and its uses.

1. understand the concepts of forking and cloning
2. issue tracking
3. understand how to use markdown
4. setting up GitHub command line on my local terminal

## __milestone 2__ :pushpin:
understanding the command line in Ubuntu Linux
find a suitable workflow program for my project

## __milestone 3__ :pushpin:
find more application with python as a programming language
1. increase my proficiency in the language

## __milestone 4__ :pushpin:
visualize data on an ongoing project here at ICIPE

1. align with an ongoing project and help the team analyze and visualize the data they’ve collected.

## __milestone 5__ :pushpin:

Identify the types of sequences I would like my library to query 

1. nucleic acid(DNA/RNA) or protein sequences
2. types of organisms or viruses to focus on.

## __milestone 6__ :pushpin:
fetch model nucleic acid and/or proteomic sequences that will be included in the repository for my library

## __milestone 7__ :pushpin:
identify which repository my library will use to call sequences

## __milestone 8__ :pushpin:
generate useful functions that will allow for manipulation of collected data
1. A function to call sequences from the selected repository
2. A function to subset data if necessary
3. A function to create phylogenetic relationships
4. A function to run different types of alignments(pairwise, multiple sequence alignment, global and local)
