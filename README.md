# Tesis

## Herramientas
Editor de codigo **VSCode** disponible en https://code.visualstudio.com/Download
Compilador **Strawberry Perl** disponible en https://strawberryperl.com/
Fuente **TeX Gyre Termes** (muy similar a New Times Roman) disponible en la web
Distribucion TeX/LaTeX **MiKTeK** disponible en https://miktex.org/download
Extension de VSCode **LaTex Workshop** de James Yu disponible en https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop

## Guia de instalacion
1. Instalar las herramientas
2. En el editor de codigo, abrir la configuracion de usuario "Open Users Settings (JSON)"
Pegar el siguiente codigo:
"latex-workshop.latex.recipes": [
    {
      "name": "latexmk (lualatex)",
      "tools": [
        "lualatexmk"
      ]
    },
    {
      "name": "latexmk",
      "tools": [
        "latexmk"
      ]
    },
    {
      "name": "latexmk (latexmkrc)",
      "tools": [
        "latexmk_rconly"
      ]
    },
    {
      "name": "latexmk (xelatex)",
      "tools": [
        "xelatexmk"
      ]
    },
    {
      "name": "pdflatex -> bibtex -> pdflatex * 2",
      "tools": [
        "pdflatex",
        "bibtex",
        "pdflatex",
        "pdflatex"
      ]
    },
    {
      "name": "Compile Rnw files",
      "tools": [
        "rnw2tex",
        "latexmk"
      ]
    },
    {
      "name": "Compile Jnw files",
      "tools": [
        "jnw2tex",
        "latexmk"
      ]
    },
    {
      "name": "Compile Pnw files",
      "tools": [
        "pnw2tex",
        "latexmk"
      ]
    },
    {
      "name": "tectonic",
      "tools": [
        "tectonic"
      ]
    }
  ]
  }


Por defecto, se compilara en *latexmk (lualatex)*
3. Aceptar la instalacion de los paquetes de la UI de MikTeX