# malab-exportfig

This is Matlab function to export figure by your rules.

### Usage
1. Put "exportfig.m" on your directory.
2. Plot your figure. You can use subplot figures.
3. Select your figure window.
4. Write on console "exportfig('./fig','pdf',[800 600])" and run.
5. Figure window is resized, and  "fig.pdf" of 800x600 px is in current directory.

### Function
```
exportfig(filename,format, m)
exportfig(filename,format, m, type )
```
* filename : filename without format name.
* format : image format including .eps, .pdf, .tiff, etc.
* m : size or aspect ratio of image.
* type: export format; 'TeX', 'TeX*', 'Slides' and 'Poster'.

### Rules
* TeX and TeX*
* Rules for LaTeX figure.

#### TeX rule is fit following figure environments of LaTeX.
```TeX
\begin{figure}[tbp]
	\centering
	\includegraphics[width=\linewidth]{fig.pdf}
	\caption{default
	\label{default}
	}
\end{figure}
```
####


#### TeX* rule is fit following figure* environments of LaTeX.
```TeX
\begin{figure*}[tbp]
	\centering
	\includegraphics[width=\linewidth]{fig.pdf}
	\caption{default
	\label{default}
	}
\end{figure*}
```
####
