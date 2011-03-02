# The semantic package

This is a mirror of the LaTeX semantic package, found on CTAN here:
[http://www.ctan.org/pub/tex-archive/macros/latex/contrib/semantic/](http://www.ctan.org/pub/tex-archive/macros/latex/contrib/semantic/)

The package is © 1995--2002 Peter Møller Neergaard and Arne John
Glenstrup. I have added one patch, which means that any \comp or \eval
environment correctly uses \compsymbol or \evalsymbol, so that these
can be changed inside a document. 

For example:

    \renewcommand{\compsymbol}[1][]{\ensuremath{\mathcal{Z}^{#1}}}
    \[
    \comp{C1 ; C2}{d} = \mathtt{d’} \quad
      \texttt{if $\comp{C1}{d} = \mathtt{d’’}$ and
        $\comp{C2}{d’’} = \mathtt{d’}$}
    \]

will use a `\mathcal{Z}` as the command symbol.