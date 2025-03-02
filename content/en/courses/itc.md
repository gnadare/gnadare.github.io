---
title: Introduction to Theory of Computation
summary: '<p style="margin-bottom:0.5cm;">This class deals with fundamental questions: what is computable, 
what is not? What is provable and what not? What is computable 
with feasible effort. The concrete example ‘can RSA be broken with 
reasonable computation time?’ shows, that such fundamental 
questions have enormous practical importance.</p>'
tags:
  - Introduction to Theory of Computation 
date: '2024-02-18T00:00:00Z'
publishDate: '2018-01-01T00:00:00Z'
show_date: false

# Optional external URL for project (replaces project detail page).
external_link: ''

#image:
#  caption: Photo by rawpixel on Unsplash
#  focal_point: Smart

links:
 # - icon: twitter
 #   icon_pack: fab
 #   name: Follow
 #   url: https://twitter.com/georgecushen
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ''
---

This class deals with fundamental questions: what is computable, 
what is not? What is provable and what not? What is computable 
with feasible effort. The concrete example ‘can RSA be broken with 
reasonable computation time?’ shows, that such fundamental 
questions have enormous practical importance.

Although we will be dealing with a very wide range of questions for the 
better half of the lectures, we are forced to rely on only two proof 
techniques: diagonalization and simulation theorems between 
computational models. We simply do not have other techniques 
which work (for now, but that is the case since many decades).

Planned course content by weeks:

1) Regular expressions, finite automata and 
nondeterminism.
2) Context free languages and pushdown automata.
3) Context sensitive languages, type-0 
languages and Turing machines.
4) Recursive functions, computability and 
decidability.
5) Undecidable problems and the recursion 
theorem.
6) Proof Systems.
7) Gödel’s incompleteness theorems.
8) Turing machine complexity classes.
9) Complexity hierarchies.
10) Speed up and Gap theorem.
11) NP completeness.
12) More about complete problems.
13) Time versus space.
14) Determinism versus nondeterminism.
15) Applications of Kolmogorov complexity.

During these lectures, we will cover fundamental results present in a more conventional 
treatment of the subject as well. In particular we will treat: The Recursion Theorem,
the two fundamental incompleteness theorems of Gödel, the speed up and gap theorems of Manuel Blum
and Allan Borodin, two fundamental separation theorems between the classic 
complexity classes of complexity theory, Applications of Kolmogorov complexity.

Literature used:

<ul style="list-style-type:disc;">
<li> <i>Introduction to the Theory of Computation.</i> Sipser M.,
Edition	3, engage Learning, (ISBN 1133187811; 9781133187813), (2012).</li>
<li> <i>Formal Languages and Their Relation to Automata.</i> Hopcroft, J. E.; Ullman, J. D., Addison-Wesley Series in Computer Science and Information Processing. Reading, Mass. etc.: Addison-Wesley Publishing Company. X, 242 p. (1969). </li>
<li> <i>Compilers. Principles, techniques, and tools.</i> 
Aho, Alfred V.; Lam, Monica S.; Sethi, Ravi; Ullman, Jeffrey D., Edition 2, Boston, MA: Pearson/Addison Wesley (ISBN 9780321486813; 9780321491695). xxiv, 1009 p. (2007). 
Because of its cover commonly known as ‘the dragon book.’</li>
<li><i>Komplexitaetstheorie.</i> Paul W., Teubner 
(1978). It is in German and out of print, but I am 
optimistic that the slides will reflect the author’s 
intentions fairly well.</li>
<li><i>Various original articles.</i></li>
</ul>

## Administration for 2025 class

The course is held on Tuesdays at 17:00-18:50 and Wednesdays 16:00-16:50. Please check your calendar for weekly updates. The location is auditorium A1 at KIU Campus. Slides and weekly exercises are available in the "Class Material" folder on the course channel in MS Teams.

Lectures are also recorded and uploaded to YouTube. Below is the playlist.
{{< youtubepl id="PL1GlRliRCb0ulFfblvMFxBk8bx_ZhlLv8" >}}

What actually happens in class is usually different from what was intended. Here, I will outline for students what was actually covered and where to find the material.

**Week 1** - Regular expressions, Finite Automata. Slides: TCS-1.

<!--
**Week 2** - Nondeterministic finite automata, Pumping Lemma for regular languages. Slides: TCS-2.

**Week 3** - Minimal DFA, Chomsky hierarchy of grammars. Slides: TCS-3, first part of TCS-4.
<ul style="list-style-type:disc;">
<li> For minimal DFA, you can also check out this very nice <a href='https://www.informatik.uni-bremen.de/agbs/lehre/ss05/pi2/hintergrund/minimize_dfa.pdf'>notes</a> by Jan Peleska.</li>
</ul>

**Week 4** - Pumping Lemma for context free grammars, Chomsky normal form, nondeterministic pushdown automata. Slides: second part of TCS-4, first part of TCS-5. 
<ul style="list-style-type:disc;">
<li> Note: TCS-6 is left out! However, you are free to review it and ask questions.</li>
</ul>

**Week 5** - Finished proofs that nondeterministic pushdown automata recognize context free languages; countable sets, primitive recursive functions, diagonal arguments. Slides: second part of TCS-5, first part of TCS-7. 

**Week 6** - Bounded and unbounded minimization, $\mu$-recursive functions; $k$-tape Turing machines. Slides: second part of TCS-7, first part of TCS-8. 

**Week 7** - Computing $\mu$-recursive functions by regular $k$-tape Turing machines. Simulating $k$-tape Turing machines by $1$-tape Turing Machines. Slides: second part of TCS-8, first part of TCS-9 (second part of TCS-9 will not be covered). 
<ul style="list-style-type:disc;">
<li> Note: next week is the midterm week.</li>
</ul>

**Week 8** - Midterm. As seen in Figure 1, midterm was easy! {{< figure src="Midterm_ITC_2024.jpg" caption="Grade distribution for the midterm." numbered="true" >}}

**Week 9** - Simulation of Turing Machines by recursive functions. Slides: TCS-10. 

**Week 10** - Non-computable functions. Gödelisation. Halting problem. Rice's Theorem. Recursively enumerable languages. Slides: TCS-11. 

**Week 11** - Proof systems. Proof system for elementary number theory. Slides: TCS-12. 

**Week 12** - The two Gödel's incompleteness theorems. Slides: TCS-13.

**Week 13** - Computational resources: time and space. Deterministic complexity classes and their equivalent definitions. Time and space bounds for the 1 and 2-tape universal Turing machine. Slides: almost finished TCS-14.

**Week 14** - Time and space hierarchy theorems. Kolmogorov complexity. Slides: finished TCS-14, first half of TCS-15.

**Week 15** - Non time constructable functions. Language not acceptable in time less than $o(n^2)$. Non deterministic Turing machine and corresponding complexity classes. Linear Bounded Automata. Slides: finished TCS-15, some parts of TCS-16.

 Figure 2 shows the final distribution of points for the course after all the exams. {{< figure src="Fin_Gr_ITC_2024.jpg" caption="Final grade distribution for the course." numbered="true" >}}
 -->