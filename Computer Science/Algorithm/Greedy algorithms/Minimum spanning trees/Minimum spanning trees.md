```tikz
\begin{document}
\begin{tikzpicture}
    \node[circle,draw] (A) at (0,2) {A};
    \node[circle,draw] (B) at (0,0) {B};
    \node[circle,draw] (C) at (3,2) {C};
    \node[circle,draw] (D) at (3,0) {D};
    \node[circle,draw] (E) at (6,2) {E};
    \node[circle,draw] (F) at (6,0) {F};

	\draw (A) -- node[above]{1} (C);
	\draw (A) -- node[pos=0.2, shift={(0,-0.3)}]{3} (D);
	\draw (A) -- node[left]{4} (B);
	\draw (B) -- node[below]{4} (D);
	\draw (C) -- node[pos=0.2, shift={(0,-0.3)}]{4} (B);
	\draw (C) -- node[right]{2} (D);
	\draw (C) -- node[midway, above]{4} (F);
	\draw (D) -- node[below]{6} (F);
	\draw (F) -- node[right]{5} (E);

\end{tikzpicture}
\end{document}
```
