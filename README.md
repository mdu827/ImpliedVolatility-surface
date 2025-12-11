\documentclass[10pt,a4paper]{article}
\usepackage[margin=1.5cm]{geometry}
\usepackage{xcolor}
\usepackage{fontawesome}
\usepackage{tikz}
\usepackage{adjustbox}
\usepackage{libertine}
\usepackage[scaled=0.85]{beramono}
\usepackage{multicol}
\usepackage{graphicx}

\definecolor{titleblue}{RGB}{0, 102, 204}
\definecolor{accent}{RGB}{255, 80, 80}

\pagestyle{empty}
\setlength{\parindent}{0pt}
\setlength{\columnsep}{1.5cm}

\begin{document}

\begin{center}
{\LARGE\bfseries\sffamily\color{titleblue} 
Implied Volatility Surface Visualizer \faChartAreaChart}\\[8pt]
{\large\sffamily Interactive 3D Volatility Explorer}
\end{center}

\vspace{12pt}

\begin{multicols}{2}

{\sffamily\small
\textbf{Overview}\\
A real-time tool that builds and visualizes the full implied volatility(IV) surfaces from live options chains. Visualize volatility smile/skew and term structure instantly for any ticker.

\vspace{8pt}
\textbf{Key Features}
\begin{itemize}
    \item Interactive 3D surface (Plotly)
    \item Strike and Moneyness display modes
    \item Plot volatility heatmap
    \item Support trade securities like stocks/ETFs etc..(e.g. SPY, AAPL, TSLA, PLTR)
    \item Live data via yfinance 
    \item One-click export (PNG/PDF)
\end{itemize}

\columnbreak

\textbf{Tech Stack}\\
Python • Streamlit • Plotly • Pandas • NumPy • yfinance
\\
\newline
{\small \quad Live access: \texttt{https://implied-vol-surface.streamlit.app} (might take 1-2 min to wake)}\\[4pt]

\end{multicols}

\vspace{10pt}

\begin{center}
\begin{adjustbox}{width=0.92\textwidth}
\includegraphics[width=\linewidth]{img/spy_plot.png}
\end{adjustbox}
\\
{\small e.g. Implied Volatility Surface for SPY}
\end{center}

\begin{center}
\begin{adjustbox}{width=0.92\textwidth}
\includegraphics[width=\linewidth]{img/pltr_plot_moneyness.png}
\end{adjustbox}
\\
{\small e.g. Implied Volatility Surface for PLTR with moneyness}
\end{center}

\begin{center}
\begin{tikzpicture}
    \node[fill=titleblue, text=white, rounded corners=4pt, minimum width=5cm, minimum height=0.8cm] 
         {\quad \textbf{github.com/mdu827/ImpliedVolatility-surface}};
\end{tikzpicture}
\\
\begin{tikzpicture}
    \node[fill=titleblue, text=white, rounded corners=4pt, minimum width=5cm, minimum height=0.8cm] 
         {\quad \textbf{http://t.me/vespasianvindex}};
\end{tikzpicture}
\end{center}

\end{document}
