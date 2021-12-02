---
documentclass: extarticle
fontsize: 14pt
title: |
    My Title\footnote{
    My thanks
    }
author: |
    My Name\footnote{
    My Place.
    ORCID: \href{https://orcid.org/XXX}{\texttt{XXX}}.
    Email: \href{mailto:XXX}{\texttt{XXX}}
    }
header-includes: |
    \usepackage[T1]{fontenc}
    \usepackage{natbib}
    \usepackage{hyperref}
    \definecolor{darkblue}{rgb}{0.0,0.0,0.3}
    \hypersetup{colorlinks=true, breaklinks=true, citecolor= darkblue, linkcolor=darkblue, urlcolor=darkblue}
    \usepackage[document]{ragged2e}
    \usepackage{babel}
---

Cite:

> *Citation*

---

```
@misc{XXX,
    author       = "",
    title        = "",
    howpublished = "",
    note         = "",
    year         = "",
}
```

\input{count.txt}

\newpage
# Section I

blah blah [@example]

\newpage

# Bibliography
