# 🏝 DesertIslandJulia 🏝

A list of resources about the Julia language

## References

### Installation

- [Classical setup from individual installer](https://julialang.org/downloads/)

- Setup from [Juliaup](https://github.com/JuliaLang/juliaup)

  **Note:** under Windows but access denied to the Windows store follow the instructions provided [here](https://discourse.julialang.org/t/looking-for-feedback-from-users-that-currently-cant-install-juliaup-from-the-windows-store/85507), namely

    1. Download [https://install.julialang.org/Julia.appinstaller](https://install.julialang.org/Julia.appinstaller)

    1. Execute the code under Powershell

       ```shell
       PS [path] Add-AppxPackage -AppInstallerFile Julia.appinstaller
       ```

### Websites

- [Julia documentation](https://docs.julialang.org/)
- [Modern Numerical Computing](http://courses.csail.mit.edu/18.337/2018/) (MIT 18.337/6.338)
- [Multidimensional algorithms and iteration](https://julialang.org/blog/2016/02/iteration/)
- [Type-dispatch-design ≠ object-oriented programming language](http://www.stochasticlifestyle.com/type-dispatch-design-post-object-oriented-programming-julia/)

### Videos

- [Intro to Julia tutorial (version 1.0) by Jane Herriman](https://youtu.be/8h8rQyEpiZA)
- [The Unreasonable Effectiveness of Multiple Dispatch](https://www.youtube.com/watch?v=kc9HwsxE1OY)
- [Developing Julia Packages](https://youtu.be/QVmU29rCjaA)
- [Automatic Differentiation with Julia](https://youtu.be/vAp6nUMrKYg)
- [State of SciML in 2022](https://www.youtube.com/watch?v=eSeY4K4bITI&t=14s)
- [Intro to solving differential equations in Julia](https://www.youtube.com/watch?v=KPEqYtEd-zY)

### Books

#### Julia High Performance

[Link to publisher](https://juliahighperformance.com/)

<details>
<summary>Abstract</summary>

> The Julia programming language has brought an innovative new approach to
> scientific computing, promising a combination of performance and productivity
> that is not usually available in the current set of languages that is commonly
> used. In solving the two- language problem, it has seen tremendous growth both
> in academia and industry. It has been used in domains from robotics,
> astronomy, and physics, to insurance and trading. It has particular relevance
> in the area of machine learning, with increasing use for the emerging field of
> differentiable computing.

> Most new developers are attracted to the language due to its promise of high
> performance. This book shows you how and why that is possible. We talk about
> the design choices of the language's creators that allow such a
> high-performance compiler to be built. We also show you the steps that you, as
> an application developer, can take to ensure the highest possible performance
> for your code. We also tell you the ways in which your code can work with the
> compiler and runtime to fully utilize your hardware to the greatest extent
> possible.

> This book is for the beginner and intermediate Julia developer who wants to
> fully leverage Julia's promise of performance with productivity. We assume you
> are proficient with one or more programming languages and have some
> familiarity with Julia's syntax. We do not expect you to be expert Julia
> programmers yet but assume that you have written small Julia programs, or that
> you have taken an introductory course on the language.

</details>

#### Hands-On Design Patterns and Best Practices with Julia

[Link to publisher](https://www.packtpub.com/product/hands-on-design-patterns-and-best-practices-with-julia/9781838648817)

<details>
<summary>Abstract</summary>

> Design patterns are fundamental techniques for developing reusable and
> maintainable code. They provide a set of proven solutions that allow
> developers to solve problems in software development quickly. This book will
> demonstrate how to leverage design patterns with real-world applications.

> Starting with an overview of design patterns and best practices in application
> design, you'll learn about some of the most fundamental Julia features such as
> modules, data types, functions/interfaces, and metaprogramming. You'll then
> get to grips with the modern Julia design patterns for building large-scale
> applications with a focus on performance, reusability, robustness, and
> maintainability. The book also covers anti-patterns and how to avoid common
> mistakes and pitfalls in development. You'll see how traditional
> object-oriented patterns can be implemented differently and more effectively
> in Julia. Finally, you'll explore various use cases and examples, such as how
> expert Julia developers use design patterns in their open source packages.

> By the end of this Julia programming book, you'll have learned methods to
> improve software design, extensibility, and reusability, and be able to use
> design patterns efficiently to overcome common challenges in software
> development.

</details>

### Jupyter notebooks

- [JuliaBoxTutorials by Jane Herriman](https://github.com/xorJane/JuliaBoxTutorials)

## Libraries

See also the following lists

- [Packages all Julians should know about?](https://discourse.julialang.org/t/packages-all-julians-should-know-about/88099) (Julia discourse)

#### General purpose

- [StaticArrays](https://github.com/JuliaArrays/StaticArrays.jl):
  Statically sized arrays for Julia
- [CxxWrap](https://youtu.be/u7IaXwKSUU0): Creation of Julia packages relying on
  C++ libraries (equivalent to `Boost.Python` or `pybind11` for Python)

#### Documentation

- [Documenter](https://github.com/JuliaDocs/Documenter.jl.git): A documentation generator for Julia.
- [DocStrings](https://github.com/miguelraz/DoctorDocstrings.jl.git): Diagnose the missing docstrings in your package. Copy paste from your REPL the smart inputs straight into your docstrings.

#### Plotting

- [Plots](http://docs.juliaplots.org/latest/) – powerful convenience for
  visualization in Julia.
- [Makie](http://makie.juliaplots.org/stable/) is a high-performance,
  extendable, and multi-platform plotting ecosystem for the Julia programming
  language.
- [PGFPlotsX](https://kristofferc.github.io/PGFPlotsX.jl/stable/) is a Julia
  package for creating publication quality figures using the LaTeX library
  PGFPlots as the backend. See also [this
  video](https://www.youtube.com/watch?v=XHJ-u7PgBs8).

#### Graphics

- [JuliaGraphics](https://github.com/JuliaGraphics)
- [Compose.jl](https://github.com/GiovineItalia/Compose.jl) is a vector graphics
  library for Julia. It forms the basis for the statistical graphics system
  [Gadfly](https://github.com/GiovineItalia/Gadfly.jl).
- [Cairo.jl](https://github.com/JuliaGraphics/Cairo.jl) – Bindings to the Cairo
  graphics library
- [ElectronDisplay.jl](https://github.com/queryverse/ElectronDisplay.jl)
  provides a display for figures, plots and tables. When you load the package,
  it will push a new display onto the julia display stack and from then on it
  will display any value that can be rendered as png, svg, vega, vega-lite or
  plotly in an electron based window. This is especially handy when one works on
  the REPL and wants plots or tables to show up in a nice window.

#### Julia 💓 LaTeX

- [LaTeXStrings](https://github.com/stevengj/LaTeXStrings.jl) – This is a small
  package to make it easier to type LaTeX equations in string literals in the
  Julia language, written by Steven G. Johnson.
- [Latexify.jl](https://github.com/korsbo/Latexify.jl) – This is a package for
  generating LaTeX maths from julia objects.
- [MathTeXEngine.jl](https://github.com/Kolaru/MathTeXEngine.jl/) – This is a
  work in progress package aimed at providing a pure Julia engine for LaTeX math
  mode. It is composed of two main parts: a LaTeX parser and a LaTeX engine,
  both only for LaTeX math mode. **Note:** “Currently the only font set
  supported is Computer Modern.”
- [juliaplots](https://github.com/sisl/juliaplots.sty): This package makes it
  easy to integrate Julia code and plots into LaTeX documents

#### Publishing

- [Weave.jl](https://github.com/JunoLab/Weave.jl) is a scientific report
  generator/literate programming tool for the
  [Julia programming language](https://julialang.org/). It resembles
  [Pweave](http://mpastell.com/pweave), [knitr](https://yihui.org/knitr/),
  [R Markdown](https://rmarkdown.rstudio.com/), and
  [Sweave](https://stat.ethz.ch/R-manual/R-patched/library/utils/doc/Sweave.pdf).
- [Franklin.jl](https://franklinjl.org/) is a simple, customisable static site
  generator oriented towards technical blogging and light, fast-loading pages.

#### Rich text output and text-based user interfaces (TUI)

- [Term.jl](https://github.com/FedeClaudi/Term.jl) is a package inspired by WIll
  McGougan’s [rich](https://github.com/Textualize/rich) package in Python to
  produce stylized, structured output for your terminal, in Julia.

#### General scientific libraries

- [SciML](https://github.com/SciML) gathers many libraries of scientific calculation
  such as
   - [DifferentialEquations.jl](https://github.com/SciML/DifferentialEquations.jl)
     for solving differential equations.
   - [Symbolics.jl](https://github.com/JuliaSymbolics/Symbolics.jl) is a fast
     and modern Computer Algebra System (CAS). Note that this library aims at
     providing expressions finally dedicated to numerical computation and not
     pure formal computation.
   - [ModelingToolkit.jl](https://github.com/SciML/ModelingToolkit.jl) is a
     modeling framework for high-performance symbolic-numeric computation in
     scientific computing and scientific machine learning.
   - [GalacticOptim.jl](https://github.com/SciML/GalacticOptim.jl) is a package
     with a scope that is beyond your normal global optimization package.
     GalacticOptim.jl seeks to bring together all of the optimization packages
     it can find, local and global, into one unified Julia interface.

#### Finite elements

- [JuAFEM.jl](https://kristofferc.github.io/JuAFEM.jl/latest/) is a finite
  element toolbox that provides functionalities to implement finite element
  analysis in Julia.
- [Gridap.jl](https://gridap.github.io/Gridap.jl/stable/) provides a set of
  tools for the grid-based approximation of partial differential equations
  (PDEs) written in the Julia programming language. The main motivation behind
  the development of this library is to provide an easy-to-use framework for the
  development of complex PDE solvers in a dynamically typed style without
  sacrificing the performance of statically typed languages. The library
  currently supports linear and nonlinear PDE systems for scalar and vector
  fields, single and multi-field problems, conforming and nonconforming finite
  element discretizations, on structured and unstructured meshes of simplices
  and hexahedra.

#### Optimization

- [JuMP.jl](https://jump.dev/) offers a modelling language for mathematical
  optimization.  It interacts with various convex optimization solvers for
  solving linear programming (LP), second-order cone programming (SOCP),
  semi-definite programming (SDP), etc.

#### Automatic differentiation

- [JuliaDiff](https://github.com/JuliaDiff): Differentiation Tools in Julia.
- [Zygote.jl](https://github.com/FluxML/Zygote.jl) provides source-to-source
  automatic differentiation (AD) in Julia, and is the next-gen AD system for the
  [Flux](https://github.com/FluxML/Flux.jl) differentiable programming framework.

#### Others

- [BifurcationKit.jl](https://github.com/rveltz/BifurcationKit.jl) aims at
  performing **automatic bifurcation analysis** of large dimensional equations
  F(u, λ)=0 where λ∈ℝ by taking advantage of iterative methods, sparse
  formulation and specific hardwares (e.g. GPU).


### Sources of inspiration

#### Python

#### Maple

- [tens3d and tenssurf](http://jean.garrigues.perso.centrale-marseille.fr/tens3d.html):
  Maple and Mathematica packages for tensor calculation (including
  variant-covariant, Christoffel coefficients, differential operators…)

<!-- Local Variables: -->
<!-- fill-column: 80 -->
<!-- End: -->
