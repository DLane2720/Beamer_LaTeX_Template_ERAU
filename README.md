# ERAU BEAMER PRESENTATION TEMPLATE - GETTING STARTED


This template creates professional 16:9 presentations with ERAU branding.

# COMPILING YOUR PRESENTATION

To generate a PDF from your presentation:

    pdflatex slide.tex

Or use your preferred LaTeX editor (TeXShop, Overleaf, etc.)

# CUSTOMIZING YOUR PRESENTATION

## BASIC INFORMATION (lines 10-14 in slide.tex)

   \author{Instructor Name}          <- Your name
   \title{Course Title}               <- Course number/title (shows in footer)
   \subtitle{Name of Slide Deck}     <- Module/lecture topic (footer center)
   \institute{Embry-Riddle...}       <- Your institution
   \date{\today}                      <- Date (or use specific: {Jan 15, 2024})

   The title appears in the left footer, subtitle in center, page numbers right.

# ADDING SECTIONS

Sections create automatic table of contents entries:

    \section{Introduction}
    \section{Main Topic}
    \section{Conclusion}

Each section automatically gets a TOC slide before it begins.

# ADDING SLIDES

Basic slide with title:

    \begin{frame}{Slide Title Here}
        Your content goes here
    \end{frame}

Slide without title:

    \begin{frame}
        Your content goes here
    \end{frame}

Slide with bullet points:

    \begin{frame}{My Topic}
        \begin{itemize}
            \item First point
            \item Second point
            \item Third point
        \end{itemize}
    \end{frame}

Slide with numbered list:

    \begin{frame}{Steps}
        \begin{enumerate}
            \item First step
            \item Second step
            \item Third step
        \end{enumerate}
    \end{frame}

# ADDING SUBSECTIONS (OPTIONAL)

For more detailed organization:

    \section{Main Topic}
    \subsection{Subtopic A}
    \subsection{Subtopic B}

# ADDING IMAGES

Place images in the pic/ folder, then:

    \begin{frame}{Image Example}
        \begin{figure}
            \centering
            \includegraphics[width=0.6\linewidth]{pic/yourimage.png}
            \caption{Image caption}
        \end{figure}
    \end{frame}

Adjust width with values like: 0.3, 0.5, 0.8, etc. (fraction of slide width)

# COLORS & BRANDING

The template uses official ERAU colors:
- Dark Blue (#003366) - Headers, structural elements
- Gold (#FFCC00) - Accent color (available if needed)
- Light Grey (#CCCCCC) - Block backgrounds

To customize colors, edit ERAU.sty (lines 88-93)

# NEED MORE HELP?

- Beamer documentation: https://ctan.org/pkg/beamer
- LaTeX basics: https://www.overleaf.com/learn

For template issues, check slide.tex and ERAU.sty for examples.
