# cv
%-------------------------
% Resume in Latex
% Author : Sourabh Bajaj + some brand new features from Mary Feofanova
% Website: https://github.com/sb2nov/resume
% License : MIT
%------------------------

\documentclass[letterpaper,10pt]{article}

\usepackage{makecell}
\usepackage[link=off]{phonenumbers}

\usepackage{latexsym}
\usepackage[empty]{fullpage}
\usepackage{titlesec}
\usepackage{marvosym}
\usepackage[usenames,dvipsnames]{color}
\usepackage{verbatim}
\usepackage{enumitem}
\usepackage[pdftex]{hyperref}
\usepackage{fancyhdr}


\pagestyle{fancy}
\fancyhf{} % clear all header and footer fields
\fancyfoot{}
\renewcommand{\headrulewidth}{0pt}
\renewcommand{\footrulewidth}{0pt}
\usepackage[margin=0.3in]{geometry}
% Adjust margins
\addtolength{\oddsidemargin}{-0.0in}
\addtolength{\evensidemargin}{-0.0in}
\addtolength{\textwidth}{0in}
\addtolength{\topmargin}{20pt}
\addtolength{\textheight}{0.0in}

\urlstyle{same}

\usepackage{xcolor}% http://ctan.org/pkg/xcolor
\usepackage{hyperref}% http://ctan.org/pkg/hyperref
\hypersetup{
  colorlinks=true,
  linkcolor=blue!50!red,
  linkbordercolor=red,
  urlcolor=blue!70!black
}

\raggedbottom
\raggedright
\setlength{\tabcolsep}{0in}

% Sections formatting
\titleformat{\section}{
  \vspace{-10pt}\scshape\raggedright\large
}{}{0em}{}[\color{black}\titlerule \vspace{-7pt}]

%-------------------------
% Custom commands
\def \ifempty#1{\def\temp{#1} \ifx\temp\empty }

\newcommand{\resumeItem}[2]{
  \item\small{
  	\ifempty{#1}#2\else\textbf{#1}{: #2 \vspace{-2pt}}\fi
  }
}

\usepackage[dvipsnames]{xcolor}
\definecolor{mygray}{gray}{0}
\usepackage{fancybox}

\usepackage{lmodern}
\usepackage{tikz}

% Style definition
\tikzset{rndblock/.style={rounded corners,rectangle,draw,outer sep=0pt}}

% Command Definition
% 1 optional to customize the aspect, 2 mandatory: text to be framed
\newcommand{\tframed}[2][]{\tikz[baseline=(h.base)]\node[rndblock,#1] (h) {\color{black}{#2}};}

\newcommand*{\mystrut}{\rule[-0.2\baselineskip]{0pt}{0.8\baselineskip}}
\newcommand{\skill}[1]{\tframed[lightgray]{\mystrut#1}}


\newcommand{\resumeSubheading}[4]{
  \vspace{-1pt}\item
    \begin{tabular*}{0.97\textwidth}{l@{\extracolsep{\fill}}r}
      \textbf{#1} & \textcolor{mygray}{#2} \\
      \textit{\small#3} & \textcolor{mygray}{\textit{\small #4}} \\
    \end{tabular*}\vspace{-5pt}
}

\newcommand{\resumeExpSubheading}[5]{
  \vspace{-1pt}\item
    \begin{tabular*}{0.97\textwidth}{l@{\extracolsep{\fill}}r}
      \textbf{#1}  & \textcolor{mygray}{#2} \\
      \textit{\small#3} & \textcolor{mygray}{\textit{\small #4}} \\
      {\scriptsize#5}
    \end{tabular*}\vspace{4pt}
}

\newcommand{\resumeProjSubheading}[4]{
  \vspace{-1pt}\item
    \begin{tabular*}{0.97\textwidth}{l@{\extracolsep{\fill}}r}
      \textbf{#1}  & \textcolor{mygray}{#2} \\
      \scriptsize {#3} & \textcolor{mygray}{\textit{\small #4}} \\
    \end{tabular*}\vspace{4pt}
}

\newcommand{\resumeSubItem}[2]{\resumeItem{#1}{#2}\vspace{-4pt}}

\renewcommand{\labelitemii}{$\circ$}

\newcommand{\resumeSubHeadingListStart}{\begin{itemize}[leftmargin=*]}
\newcommand{\resumeSubHeadingListEnd}{\end{itemize}}
\newcommand{\resumeItemListStart}{\begin{itemize}[leftmargin=0.2in]}
\newcommand{\resumeItemListEnd}{\end{itemize}\vspace{-5pt}}

\usepackage{changepage}
\newcommand{\resumeDesc}[1]{\begin{adjustwidth}{5pt}{0pt}\vspace{-2pt}{\small{#1}}\end{adjustwidth}}

%-------------------------------------------
%%%%%%  CV STARTS HERE  %%%%%%%%%%%%%%%%%%%%%%%%%%%%


\begin{document}

%----------HEADING-----------------
\begin{tabular*}{\textwidth}{l@{\extracolsep{\fill}}r}
  \textbf{\Large Zikrullo Amiri} & Email : \href{mailto:amirymax@mail.com}{amirymax@mail.com}\\
  Github: \href{https://github.com/amirymax}{amirymax} & Mobile : +7\hspace{0.5ex}921\hspace{0.5ex}648\hspace{0.5ex}08\hspace{0.5ex}72 \\
\end{tabular*}


%-----------EDUCATION-----------------
\section{Education}
  \resumeSubHeadingListStart
    \resumeSubheading
       {National Research ITMO University}{Saint Petersburg, Russia}
      {Bachelor of Science in Software Engineering}{Sep. 2021 - Jun. 2025}


      %\end{comment}
  \resumeSubHeadingListEnd



\section{Projects}
  \resumeSubHeadingListStart
    \resumeProjSubheading
      {\href{https://github.com/amirymax/abit_itmo_bot}{ITMO Abiturients’ testing Telegram bot}}{Saint Petersburg, Russia}
      {\skill{Python} \skill{SQL} \skill{Telegram}}{Apr. 2022 -- May 2022}
          \resumeDesc{
          \begin{itemize}
              \item The Bot will test pupils’ knowledge on different school subjects and mark
them in that subject.            
          \end{itemize}
          }
          
      \resumeProjSubheading
      {\href{https://github.com/amirymax/detect_gestures}{Detect Gestures}}{Saint Petersburg, Russia}
      {\skill{Python} \skill{OpenCV} \skill{Computer Vision}  }{Feb. 2022 -- Mar. 2022}
          \resumeDesc{
          \begin{itemize}
              \item Using webcam program will detect a human’s hand's motion gesture, and depending on it, performs certain actions 
              \item Real time webcam viewing     
            \end{itemize}
          }

      \resumeProjSubheading
      {\href{https://github.com/amirymax/Volume-Controller}{Volume-Controller}}{Saint Petersburg, Russia}
      {\skill{Python} \skill{OpenCV} \skill{Computer Vision}}{Jan. 2022 - Feb. 2022}
          \resumeDesc{
          \begin{itemize}
              \item Using the thumb and index finger, User is able to control the volume of sound
              \item Real time webcam viewing

          \end{itemize}
          }
    \resumeProjSubheading
      {\href{https://github.com/amirymax/snake_pygame}{Snake Game}}{Saint Petersburg, Russia}
      {\skill{Python} \skill{PyGame} \skill{OOP}}{Nov. 2022 - Dec. 2022}
          \resumeDesc{
          \begin{itemize}
              \item Snake game made to enjoy your time
              

          \end{itemize}
          }
    \resumeProjSubheading
      {\href{https://github.com/amirymax/Shooting-Man}{Goblin Shooter}}{Saint Petersburg, Russia}
      {\skill{Python} \skill{PyGame} \skill{OOP}}{Nov. 2022 - Dec. 2022}
          \resumeDesc{
          \begin{itemize}
              \item A simple shooter game made using PyGame, in which you will shot the Goblin and score points
              

          \end{itemize}
          }
  \resumeSubHeadingListEnd

\section{Achievements}
% \resumeProjSubheading
% {Republican Olympiad in Informatics}{Dushanbe, Tajikistan}
\vspace{5pt}
          \resumeSubHeadingListStart{
          \item   {\textbf{Republican Olympiad in Informatics Dushanbe, Tajikistan}} Bronze medal and  \textbf{$3^{rd}$ degree diploma}  150+ participants {25-28 Apr. 2019}
              \item {\textbf{Republican Olympiad in Informatics Dushanbe, Tajikistan}}
{Silver medal and \textbf{$2^{nd}$ degree diploma} 200+ participants} {19-23 Mar. 2021}
          }    
      \resumeSubHeadingListEnd

%--------PROGRAMMING SKILLS------------
\section{Programming Skills}
 \resumeSubHeadingListStart
   \item{
     \textbf{Languages} (experienced){: Python,  (familiar): C, C++, Java, JavaScript  }
   }\vspace{-4pt}
   \item{
     \textbf{Technologies}{: Git/GitHub, Linux (Bash), SQl}
   }
   \vspace{-4pt}
   \item{
     \textbf{Knowledge}{: Algorithms, Data Structures}
   }
 \resumeSubHeadingListEnd

\section{Languages}
 \resumeSubHeadingListStart
   \item{
     \textbf{English}: C1 Level
   }\vspace{-5pt}
   \item{
     \textbf{Russian}: Native
   }
   \vspace{-5pt}
   \item{
     \textbf{Tajik}: Native
   }
 \resumeSubHeadingListEnd


%-------------------------------------------
\end{document}
