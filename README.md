# R for the Rest of Us Demo

This repository hosts materials related to the episode of the *R for the Rest of Us* podcast I joined for in early 2025.

<!--  TODO: link to the podcast episode -->

You can install the packages I spoke about during the podcast with the following code:

``` r
# if needed:
# install.packages("pak")

pak::pak(c(
  # a library of prompts at the cursor
  "simonpcouch/pal",
  # automated unit testing
  "simonpcouch/ensure",
  # a low-friction chat interface
  "simonpcouch/gander"
))
```

* [pal](https://github.com/simonpcouch/pal) binds a library of AI assistants to a keyboard shortcut
* [ensure](https://github.com/simonpcouch/ensure) automatically drafts unit tests for R package code at the press of a keyboard shortcut
* [gander](https://github.com/simonpcouch/gander) provides a high-performance, low-friction chat interface for R

pal and ensure are mostly aimed at R package developers, while gander is especially useful for data science. For more on how these three packages are related to each other and other options for LLM code-assist for R, check out this [tidyverse blog post](https://deploy-preview-721--tidyverse-org.netlify.app/blog/2025/01/experiments-llm/).

<!-- TODO: use production link above when ready -->

In the demo, we explored this dataset using the gander addin:

``` r
library(ggplot2)

data("stackoverflow", package = "modeldata")

stackoverflow
```

> TODO: add a "completed" script reflecting where we ended up at the end of the demo
