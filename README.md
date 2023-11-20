# Identificación y caracterización de radiofuentes puntuales.

A partir de tres mosaicos de la región con coordenadas galácticas $l=[206.65, 208.10] \mathrm{deg}, b=[-18.30,-20.71] \mathrm{deg}$ centrados en las frecuencias 1440, 1820 y 884 MHz, se implementa un proceso de fotometría de apertura para identificar posibles fuentes puntuales, utlizando una apertura eliptica con dimensiones iguales al beam sintetico de cada mosaico (`id_ms_1884_v1.ipynb`). Como resultado de este procedimiento se hallan las coordenadas de las posibles fuentes puntuales. Una vez conocidas las coordendas, se realiza un match up de estas en las bases de datos astronomícas SIMBAD y NED, con el proposito de encontrar cuales de estas se encuentrán reportadas en la literatura. Las fuentes que se encuentran en las bases de datos son eliminadas de nuestra consideración. Posteriormente, las coordenadas de las fuentes no identificadas se extraen para crear un archivo de coordenadas en el formato del visualizador DS9, el cual es compatible con el visualizador del software CASA, `imview`. Se genera, nuevamente una apertura eliptica con las mismas dimensiones dle beam sintetica, para extraer el pico máximo de emisión de cada fuente puntual y valor de la razón señal ruido (rms). Una vez conocidos los valores de la densidad de flujo, y la incertidumbre asociada, de cada fuente en los tres mosaicos (ie, en las tres frecuencias centrales), se procede a encontrar el valor del índice espectral de cada fuente (`SED.ipynb`), suponiendo una emisión modelada por: $F(\nu) \propto \nu^{\alpha}$.


----

\begin{itemize}
\item mosacio 1440
\end{itemize}
