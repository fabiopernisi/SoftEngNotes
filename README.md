# SoftEngNotes
This repository contains the file with the lecture notes for the course "20875 - Software Engineering" taught in the MSc in Artificial Intelligence at Bocconi University.\
The notes have been adapted from the material provided by Professor [Laurent Poirrier](https://www.poirrier.ca/courses/softeng/). This repo contains the transcription of the notes at the link, with some small changes and with more material and text.

## Contributing
### Headers convention
The file `skeleton.txt` contains a sample latex format that includes several packages (probably all that you would ever need), including `hyperref`, to make the table of contents clickable.\
Please adopt the following convention when contributing to the latex notes:
- every Lecture represents a `section`
- every title that uses a whole slide is a `subsection`
- every title followed by some text in the same slide is a `subsubsection`
- every minor title or example is a `paragraph` (i.e. `\paragraph{minor_title}`)

Where the `\paragraph{}` command needs to be defined as follows:
```
\usepackage{titlesec}

\setcounter{secnumdepth}{4}

\titleformat{\paragraph}
{\normalfont\normalsize\bfseries}{\theparagraph}{1em}{}
\titlespacing*{\paragraph}
{0pt}{3.25ex plus 1ex minus .2ex}{1.5ex plus .2ex}
```

### Numbering, case and spacing conventions
- Sections should be numbered, i.e. no `*` after any Heading keywords (`section`, `subsection`, and so on). This will allow to have a table of contents. \
    ✅ `\section{my_section}`, `\subsection{my_subsection}`\
    ❌ `\section*{my_section}`, `\subsection*{my_subsection}`

- Every Section Should __not__ be entirely in Uppercase:\
    ✅ `\section{Code Portability}`\
    ❌ `\section{CODE PORTABILITY}`

- Every section should be preceeded by a `\newpage` command

### Cleaning and Postprocessing
Every folder `p01_output, ..., p22_output` contains a `text.txt` file with the raw outputs of the GPT4 vision model. Please include the cleaned up version of each folder `p<i>_output` with the name `text<i>.txt`.

## Progress
| file        | cleaning | additional material |
|-------------|----------|---------------------|
| Lecture 1   |   ✅     |         ❌         |
| Lecture 2   |   ✅     |         ❌         |
| Lecture 3   |   ❌     |         ❌         |
| Lecture 4   |   ❌     |         ❌         |
| Lecture 5   |   ❌     |         ❌         |
| Lecture 6   |   ✅     |         ❌         |
| Lecture 7   |   ✅     |         ❌         |
| Lecture 8   |   ✅     |         ❌         |
| Lecture 9   |   ✅     |         ❌         |
| Lecture 10  |   ✅     |         ❌         |
| Lecture 11  |   ✅     |         ❌         |
| Lecture 12  |   ✅     |         ❌         |
| Lecture 13  |   ⚙️     |         ❌         |
| Lecture 14  |   ⚙️     |         ❌         |
| Lecture 15  |   ⚙️     |         ❌         |
| Lecture 16  |   ⚙️     |         ❌         |
| Lecture 17  |   ⚙️     |         ❌         |
| Lecture 18  |   ⚙️     |         ❌         |
| Lecture 19  |   ⚙️     |         ❌         |
| Lecture 20  |   ⚙️     |         ❌         |
| Lecture 21  |   ⚙️     |         ❌         |
| Lecture 22  |   ⚙️     |         ❌         |


Here:
- ✅ the file has been cleaned/enriched according to the Contributing guidelines
- ⚙️ work in progress
- ❌ still require most of the work
