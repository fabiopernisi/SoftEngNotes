# SoftEngNotes
This repository contains the file with the lecture notes for the course "20875 - Software Engineering" taught in the MSc in Artificial Intelligence at Bocconi University.\
These notes are a student effort by Giosuè Castellano and Fabio Pernisi and are intended as a supplementary resource, not an official course guide.

The content is derived from materials provided by Professor [Laurent Poirrier](https://www.poirrier.ca/courses/softeng/) (also see the `slides` folder), with an effort to retain the original strucutre. However, we replaced images with descriptive texts and summarized or expanded coding examples for (hopefully) a better understanding. Our aim was to transform the slides into more detailed (yet concise) study materials, ideal for exam prep.

## Contributing & Repo Structure
### Headers convention
The following conventions have been adopted in the Latex source code:
- every Lecture is represented by a `section`
- every title that uses a whole slide is a `subsection`
- every title followed by some text in the same slide is a `subsubsection`
- every minor title or example is a `paragraph` (i.e. `\paragraph{minor_title}`)

Where the `\paragraph{}` command is defined as follows:
```
\usepackage{titlesec}

\setcounter{secnumdepth}{4}

\titleformat{\paragraph}
{\normalfont\normalsize\bfseries}{\theparagraph}{1em}{}
\titlespacing*{\paragraph}
{0pt}{3.25ex plus 1ex minus .2ex}{1.5ex plus .2ex}
```

### Numbering, case and spacing conventions
- Sections are numbered, i.e. no `*` after any Heading keywords (`section`, `subsection`, and so on). This allows to have a clickable table of contents. \
    ✅ `\section{my_section}`, `\subsection{my_subsection}`\
    ❌ `\section*{my_section}`, `\subsection*{my_subsection}`

- Every Section is __not__ entirely in Uppercase:\
    ✅ `\section{Code Portability}`\
    ❌ `\section{CODE PORTABILITY}`

- Every section is preceeded by a `\newpage` command

### Cleaning and Postprocessing
The `Slides2Latex` folder includes a Notebook for making requests to the GPT-4 API and stores chunks of slides as three images each.\
Inside, you'll find folders named `p01_output` through `p22_output`, each corresponding to a lecture. These contain a `text.txt` file with the raw GPT-4 outputs for the slide transcriptions. The cleaned versions (with no material added) of these outputs are in files named `text<i>.txt`, where `<i>` matches the lecture number.\
The final (cleaned + enhanced) Latex code is present in the `CompleteLectureNotes.tex` file, with `CompleteLectureNotes.pdf` being the final, compiled pdf.

## Progress
| file        | Status | 
|-------------|----------|
| Lecture 1   |   ✅     |
| Lecture 2   |   ✅     |
| Lecture 3   |   ✅     | 
| Lecture 4   |   ✅     |
| Lecture 5   |   ✅     |
| Lecture 6   |   ✅     |
| Lecture 7   |   ✅     |
| Lecture 8   |   ✅     |
| Lecture 9   |   ✅     |
| Lecture 10  |   ✅     |
| Lecture 11  |   ✅     |
| Lecture 12  |   ✅     |
| Lecture 13  |   ✅     |
| Lecture 14  |   ✅     |
| Lecture 15  |   ✅     |
| Lecture 16  |   ✅     |
| Lecture 17  |   ✅     |
| Lecture 18  |   ✅     |
| Lecture 19  |   ✅     |
| Lecture 20  |   ✅     |
| Lecture 21  |   ✅     |
| Lecture 22  |   ✅     |


Here:
- ✅ file is finished, even though furhter additions/examples are always beneficial :)
- ⚙️ The file is updated and cleaned, including all notes except images that cannot be rendered by GPT-4, with some examples (e.g. long chuncks of code) removed; it requires further additions/explanations.
- ❌ still requires most of the work
