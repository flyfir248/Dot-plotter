# Dotplot Generator
This script generates a dotplot from two sequences in FASTA format. The dotplot is a graphical representation of the similarities between two sequences.

# Requirements
**Python 3**

**NumPy**

**Matplotlib**

**argparse**

# Usage
```
python dotplot.py w s seqA seqB title output
```

where:

* w: window size
* s: stringency
* seqA: filename of the first sequence in FASTA format
* seqB: filename of the second sequence in FASTA format
* title: title of the dotplot
* output: output filename for the dotplot

# Output
The script generates two types of dotplots:

* ASCII dotplot: an ASCII art representation of the dotplot, saved in a text file with the extension .txt.
* Graphical dotplot: a graphical representation of the dotplot, saved in a PNG image file with the extension .png.

# Implementation
The script uses the dotplot() function to generate a matrix of ones and zeros representing the similarity between the two sequences. The dotplot2Ascii() function converts the matrix to an ASCII art representation, and the dotplot2Graphics() function plots the matrix as a scatter plot.

# Example
To generate a dotplot for two sequences seqA.fasta and seqB.fasta with window size 10 and stringency 5, and save the dotplot with the title My Dotplot and filename mydotplot, run:
```
python dotplot.py 10 5 seqA.fasta seqB.fasta "My Dotplot" mydotplot
```