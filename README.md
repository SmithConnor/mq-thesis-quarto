
<!-- README.md is generated from README.qmd. Please edit that file -->

# Macquarie University Thesis Quarto Template <img src="https://user-images.githubusercontent.com/15133161/200966938-ba6f8413-fa77-4ccb-b16d-d7cf14926057.png" align ="right" alt="" width ="150"/>

This project is our attempt to bring our `thesisdownmq` package to
everyone! Unlike R Markdown and our previous work on `thesisdownmq`,
Quarto doesn’t have a dependency or requirement for `R`. Quarto was
developed to be multilingual, beginning with `R`, `Python`,
`Javascript`, and `Julia`, with the idea that it will work even for
languages that don’t yet exist.

Here is a preview on what the thesis looks like:
![](https://github.com/thomas-fung/mq-thesis-quarto/assets/15133161/a3572f0c-cffb-4e0d-9b22-dd8a1c22a7a7.png)

Currently, the PDF version is fully-functional (The word, gitbook and
epub versions are developmental, have no templates behind them, and are
essentially calls to the appropriate functions via Quarto.)

Under the hood, the Reed College template was updated to ensure that
documents conform precisely to submission standards at Macquarie
University. At the same time, composition and formatting can be done
using lightweight markdown syntax, and code from your favourite language
and its output can be seamlessly included using rmarkdown.

Using Quarto has some prerequisites which are described below. To
compile PDF documents, you are going to need to have installed. It can
be downloaded for Windows at http://http://miktex.org/download and for
Mac at http://tug.org/mactex/mactex-download.html. (If you are an R
user, we recommend you to install the `tinytex` package instead.) Follow
the instructions to install the necessary packages after downloading the
(somewhat large) installer files. You may need to install a few extra
packages on your first attempt to knit as well.

An example of the thesis template can be downloaded from here:
https://github.com/thomas-fung/mq-thesis-quarto/blob/main/examples/sample.pdf.

If you are simply looking for a Macquarie University thesis LaTeX
template, you should check this out:
https://github.com/aalexei/mqthesis.

### Installing Quarto

Use the following link to install Quarto:

https://quarto.org/docs/get-started/

Notice that it should come with the more recent versions of `RStudio`.

### Installing the template from Thomas Fung’s GitHub

You can use this as a template to create a report. To do this, use the
following command in your Terminal:

``` bash
quarto use template thomas-fung/mq-thesis-quarto
```

This will install the extension and download a bunch of qmd files
(basically one per chapter) that you can use as a starting place for
your thesis.

To compile your thesis into a pdf, use the following command in your
terminal

``` bash
quarto render --to mqthesis-pdf
```

or if you are an R user, type the following command in your R console

``` bash
library(quarto)
quarto_render(output_format = "mqthesis-pdf")
```

Please notice that the file `_quarto.yml` contains all the required
`YAML` information of the document.

## How to cite

``` bibtex
@misc{mqthesisquarto2023,
  author = {Fung, Thomas},
  title = {Macquarie University Thesis Quarto Template},
  year = {2023},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/thomas-fung/mq-thesis-quarto}}
}
```

*NOTE: If you’ve used this template to write your thesis, drop me a line
at thomas.fung.dr@gmail.com and I’ll add a link to showcase it!*

### This template would satisfy the following formating requirement

#### Presentation and formatting

- in A4 pdf format
- 1.5 spacing
- meant to be printed as one-sided
- margins of at least 3cm on the left border, at least 1.5cm on the
  right border and at least 1.5cm on the top and bottom
- pages numbered consecutively

#### Preliminary pages

The preliminary pages will be organised in the following order (some
items can be removed):

- A title page with:
  - the thesis title
  - your names and degrees
  - your university department
  - date of submission/re-submission.
- a table of content
- a list of tables
- a list of figures
- an abstract
- A signed statement of originality (following this
  [template](https://students.mq.edu.au/__data/assets/word_doc/0004/1141276/statement-of-originality-example.docx))
  - **you will have to add in your own Ethics Committee approval and
    protocol number (if applicable)**
- acknowledgement
- the written component of the thesis
