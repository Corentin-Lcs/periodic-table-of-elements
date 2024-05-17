<h1 align="center">Periodic Table of Elements</h1>

The "Periodic Table of Elements" GitHub project is a comprehensive resource that features D. Mendeleev's periodic table of chemical elements. This table is a visual representation of the known chemical elements, which is organized according to their physical and chemical properties with an exhaustive legend.

> [!NOTE]  
> The source of the initial code is [here](https://texample.net/tikz/examples/periodic-table-of-chemical-elements).

<p align="center">
  <img src="https://github.com/Corentin-Lcs/periodic-table-of-elements/blob/main/Periodic_Table.jpg" alt="Periodic_Table.jpg"/>
</p>

## Usage

The `.tex` files contain the complete configuration of the tables in English and French. The families of `lanthanides` and `actinides` elements are represented outside the table, below more precisely. Currently, the dotted lines connecting the two families to the main table are ignored by the compiler (the code is commented out). To add them, remove the `%` symbol from the following lines of the file :

```tex
% Draw dotted lines connecting Lanthanide breakout to main table
  \draw (LaLu.north west) edge[dotted] (La.north west)
        (LaLu.north east) edge[dotted] (Lu.north east)
        (LaLu.south west) edge[dotted] (La.south west)
        (LaLu.south east) edge[dotted] (Lu.south east);

% Draw dotted lines connecting Actinide breakout to main table
  \draw (AcLr.north west) edge[dotted] (Ac.north west)
        (AcLr.north east) edge[dotted] (Lr.north east)
        (AcLr.south west) edge[dotted] (Ac.south west)
        (AcLr.south east) edge[dotted] (Lr.south east);
```

Here is the result (without the lines on the left, with on the right) :

<div align="center">
<img height="230em" src="https://github.com/Corentin-Lcs/periodic-table-of-elements/blob/main/Without_Lines.png"/>&nbsp;&nbsp;<img height="230em" src="https://github.com/Corentin-Lcs/periodic-table-of-elements/blob/main/With_Lines.png"/>
</div> 

## Project's Structure

```
periodic-table-of-elements/ 
├─ README.md
├─ LICENSE
├─ Periodic_Table.jpg
├─ With_Lines.png
├─ Without_Lines.png
└─ src/
   ├─ LaTeX LPPL.pdf
   ├─ EN/
   │  ├─ Periodic Table of Elements.pdf
   │  └─ Periodic_Table_of_Elements.tex
   └─ FR/
      ├─ Tableau Périodique des Éléments.pdf
      └─ Tableau_Périodique_des_Éléments.tex
```

Named `./EN/Periodic Table of Elements.pdf`, the file contains the English version of the Periodic Table of Elements and is the compiled version of `Periodic_Table_of_Elements.tex`.

Named `./FR/Tableau Périodique des Éléments.pdf`, the file contains the French version of the Periodic Table of Elements and is the compiled version of `Tableau_Périodique_des_Éléments.tex`.

## Meta

Created by [@Corentin-Lcs](https://github.com/Corentin-Lcs). Feel free to contact me !

Distributed under the GNU GPLv3 license. See [LICENSE](https://github.com/Corentin-Lcs/periodic-table-of-elements/blob/main/LICENSE) for more information.
