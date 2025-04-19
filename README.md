# cme100-python

Python version of MATLAB exercises for CME 100 at Stanford University.

Access it through our [Jupyter Book](https://enze-chen.github.io/cme100-python/)!


## For instructors

Here's what Enze's convoluted process entails (if you don't like it, feel free to use your own):
1. Clone the repo and ask Enze or Vadim for the solution Python notebooks.
1. Move the solution notebooks into their proper folders (workbook or tutorials).
1. Anytime you modify the solutions, update the `_blank` notebooks (what is actually compiled in the Jupyter Book) by running from _above_ the root folder: `python cme100-python/assets/make_blank_nb.py`.
1. Run a full build of the Jupyter Book from above the root folder: `jb build cme100-python --all`.
1. Enter the root folder and publish to GitHub pages: `ghp-import -n -p -f _build/html`.
1. Don't forget to commit+push changes as needed to keep the Github up to date (but this doesn't change what students see).
1. If you want to compile the solution notebooks as PDFs, use the `convert_pdf.py` file: 
```
python convert_pdf.py {path_to_solution_notebooks} -n {merged_pdf_name.pdf}
```