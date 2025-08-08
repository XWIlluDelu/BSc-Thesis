# LaTeX Compile Setting

I am using MikTeX and Visual Studio Code. My LaTeX Workshop settings (partially shown) are as follows:

```json
    // LaTeX Settings
    "latex-workshop.latex.tools": [
        {
            "name": "latexmk (xelatex)",
            "command": "latexmk",
            "args": [
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "-xelatex",
                "-outdir=%OUTDIR%",
                "%DOCFILE%"
            ]
        },
        {
            "name": "latexmk (pdflatex)",
            "command": "latexmk",
            "args": [
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "-pdf",
                "-outdir=%OUTDIR%",
                "%DOCFILE%"
            ]
        }
    ],
    "latex-workshop.latex.recipes": [
        {
            "name": "latexmk (xelatex)",
            "tools": [
                "latexmk (xelatex)"
            ]
        },
    ],
```
