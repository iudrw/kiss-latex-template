# Keep it simple stupid LaTex Template

There's a VSCode workspace settings file, which should allow to start writing latex right away in that editor.

## Requirements

- LaTeX distribution in system PATH. For example, TeX Live (recommended).

## Latex recipe

`
latexmk -xelatex -synctex=1 -interaction=nonstopmode -file-line-error -output-directory=.build report.tex
`

🠣

`
biber --input-directory=".build" --output-directory=".build" report
`

🠣

`
latexmk -xelatex -synctex=1 -interaction=nonstopmode -file-line-error -output-directory=.build report.tex
`
