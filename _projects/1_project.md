---
layout: page
title: Matrix Multiplication on Low-Power Processors
description: Research conducted under the supervision of Enrique Quintana and Adrian Castellon.
img: /assets/img/B3C2A0.png
importance: 1
category: work
---

## The Evolution of Matrix Multiplication Algorithms

Matrix multiplication is a core operation in mathematics, computer science, and engineering, with widespread applications in scientific computing, graphics, physics simulations, and deep learning. The computational complexity of this operation has been a major focus in algorithm research, particularly the pursuit of lowering its exponent, commonly denoted as omega (ω).

A breakthrough occurred in 1969 when Strassen dramatically reduced the exponent below the classical cubic bound, sparking a decades-long race among researchers to discover even faster algorithms. The progress is charted by a series of landmark results, especially in the early 1980s and again in the last decade. Recent advances (2020–2024) highlight how even minor improvements are now hard-won and intellectually significant.

Optimizing matrix multiplication is not only a theoretical challenge but also critical for real-world performance, especially in resource-constrained environments such as low-power processors—an area at the heart of this research project.

---

### Visual Timeline

<div class="text-center">
  <img 
    src="/assets/img/matrix_exponet_8.png" 
    alt="Timeline of Matrix Multiplication Exponent Reduction"
    class="img-fluid rounded mx-auto d-block"
    style="max-width: 1000px;"
  >
  <p class="caption">
    <em>Figure 1. Timeline of major advances in reducing the exponent of matrix multiplication (omega, ω). Each step represents a new upper bound, marking significant milestones in computational complexity theory.</em>
  </p>
</div>

---

### Historical Table of Key Results

<div style="overflow-x:auto">

<table class="table table-striped table-bordered" style="min-width:700px">
  <caption>
    <strong>Table 1.</strong> Key milestones in reducing the exponent for matrix multiplication. Lower omega values reflect more efficient algorithms and progress in both theoretical and practical computational mathematics.
  </caption>
  <thead>
    <tr>
      <th>Year</th>
      <th>Omega Bound</th>
      <th>Authors</th>
      <th>Reference</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1969</td>
      <td>2.8074</td>
      <td><strong>Volker Strassen</strong></td>
      <td><a href="https://doi.org/10.1007/BF02165411" target="_blank">Numerische Mathematik</a></td>
    </tr>
    <tr>
      <td>1978</td>
      <td>2.7960</td>
      <td><strong>Victor Pan</strong></td>
      <td><a href="https://ieeexplore.ieee.org/document/4567976" target="_blank">IEEE FOCS</a></td>
    </tr>
    <tr>
      <td>1979</td>
      <td>2.7800</td>
      <td><strong>Dario Bini, Massimo Capovani, Felice Romani</strong></td>
      <td><a href="https://doi.org/10.1016/0024-3795(79)90293-7" target="_blank">Linear Algebra Appl.</a></td>
    </tr>
    <tr>
      <td>1981</td>
      <td>2.5220</td>
      <td><strong>Arnold Schönhage</strong></td>
      <td><a href="https://doi.org/10.1137/0210032" target="_blank">SIAM J. Comput.</a></td>
    </tr>
    <tr>
      <td>1981</td>
      <td>2.5170</td>
      <td><strong>Felice Romani</strong></td>
      <td><a href="https://doi.org/10.1137/0211020" target="_blank">SIAM J. Comput.</a></td>
    </tr>
    <tr>
      <td>1981</td>
      <td>2.4960</td>
      <td><strong>Don Coppersmith, Shmuel Winograd</strong></td>
      <td><a href="https://ieeexplore.ieee.org/document/4568320" target="_blank">IEEE STOC</a></td>
    </tr>
    <tr>
      <td>1986</td>
      <td>2.4790</td>
      <td><strong>Volker Strassen</strong></td>
      <td><a href="https://doi.org/10.1007/BF01391328" target="_blank">Numerische Mathematik</a></td>
    </tr>
    <tr>
      <td>1990</td>
      <td>2.3755</td>
      <td><strong>Don Coppersmith, Shmuel Winograd</strong></td>
      <td><a href="https://doi.org/10.1007/BF02166964" target="_blank">J. Symb. Comput.</a></td>
    </tr>
    <tr>
      <td>2010</td>
      <td>2.3737</td>
      <td><strong>Andrew Stothers</strong></td>
      <td><a href="https://core.ac.uk/download/pdf/222955651.pdf" target="_blank">Thesis</a></td>
    </tr>
    <tr>
      <td>2012</td>
      <td>2.3729</td>
      <td><strong>Virginia Vassilevska Williams</strong></td>
      <td><a href="https://doi.org/10.1145/2213977.2214056" target="_blank">STOC</a></td>
    </tr>
    <tr>
      <td>2014</td>
      <td>2.3728639</td>
      <td><strong>François Le Gall</strong></td>
      <td><a href="https://arxiv.org/abs/1402.4184" target="_blank">arXiv</a></td>
    </tr>
    <tr>
      <td>2020</td>
      <td>2.3728596</td>
      <td><strong>Joshua Alman, Virginia Vassilevska Williams</strong></td>
      <td><a href="https://arxiv.org/abs/2010.05846" target="_blank">arXiv</a></td>
    </tr>
    <tr>
      <td>2022</td>
      <td>2.3718660</td>
      <td><strong>Ran Duan, Zeyu Wu, Chi Zhou</strong></td>
      <td><a href="https://arxiv.org/abs/2308.13171" target="_blank">arXiv</a></td>
    </tr>
    <tr>
      <td>2024</td>
      <td>2.3715520</td>
      <td><strong>Virginia Vassilevska Williams, Zhixian Xu, Kai Xu, Chi Zhou</strong></td>
      <td><a href="https://arxiv.org/abs/2310.05373" target="_blank">arXiv</a></td>
    </tr>
    <tr>
      <td>2024</td>
      <td>2.3713390</td>
      <td><strong>Joshua Alman, Ran Duan, Virginia Vassilevska Williams, Zhixian Xu, Kai Xu, Chi Zhou</strong></td>
      <td><a href="https://arxiv.org/abs/2403.10680" target="_blank">arXiv</a></td>
    </tr>
  </tbody>
</table>
</div>

---

*This timeline and table summarize more than fifty years of ongoing advances in one of theoretical computer science’s most fundamental questions, providing the context for this project's focus on practical, energy-efficient computation.*

