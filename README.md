1. The easiest way to run this REMARK will be to use [`conda`](https://conda.io/projects/conda/en/latest/user-guide/getting-started.html),  [`git`](https://git-scm.com/), and `bash` (or another shell scripting language) with the following commands:

```bash
git clone https://github.com/econ-ark/Aiyagari-Idiosyncratic
cd Aiyagari-Idiosyncratic
conda env update -f binder/environment.yml
bash reproduce.sh
```


2. The following graph contains main files and shows how this folder is structured.

```
.
├── Aiyagari1994QJE.ipynb
├── Aiyagari1994QJE.py
├── Aiyagari.yaml
├── binder
│   └── environment.yml
├── Data
├── README.md
├── reproduce.sh
└── Tex
    ├── Appendix
    ├── Equations
    ├── Figures
    ├── main.tex
    ├── References
    ├── Slides
    └── Tables
```

Where:
* "Aiyagari1994QJE" is the Jupyter Notebook file, which includes key features of the paper and python codes implementing to replicate the main results of the paper;
*  "Aiyagari.yaml" is a yaml file where the model is written;
* "Tex" is a folder where the .tex file is located. It includes main content, figures, tables, slides, and an appendix as a subfile.
* "reproduce.sh"  is the file which contains all codes for solving the model, generating tables and figures, saving the table in  both markdown and LaTeX languages, and re-compiling the LaTeX file each time you run the code.

