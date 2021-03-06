--- 
title: "Yet another 'R for Data Science' study guide"
author: "Bryan Shalloway"
date: "Last updated: 2019-08-13"
site: bookdown::bookdown_site
url: https\://brshallo.github.io/r4ds_solutions/
github-repo: "brshallo/r4ds_solutions"
twitter-handle: brshallo
documentclass: book
bibliography: ["book.bib"]
biblio-style: apalike
link-citations: yes
description: "Notes and solutions to Garrett Grolemund and Hadley Wickham's 'R for Data Science'"
cover-image: "/images/yards_icon.png"
output:
  bookdown::gitbook:
    css: style.css
    includes:
      after_body: 
      - "disqus.html"
    split_by: "rmd"
    number_sections: FALSE
    download: no
    config:
      edit:
        link: https\://github.com/brshallo/r4ds_solutions/edit/master/%s
        text: "Edit, fork"
      sharing:
        twitter: yes
        linkedin: yes
        facebook: no
        weibo: no
        instapaper: no
        google: no
      toc:
        before: |
          <li><a href="./">Yet another R4DS study guide</a></li>
        after: |
          <li><a href="https://github.com/rstudio/bookdown" target="blank">Published with bookdown</a></li>
---

# Purpose

<img src="./images/yards_icon.png" width="400" height="250" alt="Cover image" align="right" style="margin: 0 1em 0 1em"/>

This book contains my solutions and notes to Garrett Grolemund and Hadley Wickham's excellent book, [R for Data Science](https://r4ds.had.co.nz/) [@WickhamGrolemund2017]. *R for Data Science* (R4DS) is my go-to recommendation for people getting started in R programming, data science, or the "tidyverse".

First and foremost, this book was set-up as a resource and refresher for myself^[And as a chance to experiment with using [bookdown](https://bookdown.org/).]. If you are looking for a reliable solutions manual to check your answers as you work through R4DS, I would recommend using the solutions created and mantained by Jeffrey Arnold, [R for Data Science: Exercise Solutions](https://jrnold.github.io/r4ds-exercise-solutions/)^[Jeffrey Arnold has done an excellent job of getting concise solutions and community feedback. Learn more about his project [here](https://resources.rstudio.com/rstudio-conf-2019/solving-r-for-data-science).]. Though feel free to use *Yet another 'R for Data Science' study guide* as another point of reference^[I worked through the problems independently, so for open-ended questions you'll likely see slightly different solutions from Jeffrey Arnold's.].

## Origin

I first read and completed the exercises to R4DS in early 2017 on the tail-end of completing a Master's in Analytics program. My second time going through R4DS came in early 2018 when myself and Stephen Kimel organized an internal "R for Data Science" study group with our colleagues^[[Here](https://youtu.be/eeCELJNWEuw) is part of an internal talk I gave plugging "tidy" data science, and implicitly, our R4DS study group.]. In June of 2019 I published my solutions and notes into this book.

## Organization and features

*Chapters start with the following:*

\BeginKnitrBlock{rmdimportant}<div class="rmdimportant">* A list of "Key exercises" deemed good for discussion in a study group  </div>\EndKnitrBlock{rmdimportant}
\BeginKnitrBlock{rmdtip}<div class="rmdtip">* A list of functions (and sometimes notes) from the chapter^[When functions show up in multiple locations I typically only note them the first time they appear.]  </div>\EndKnitrBlock{rmdtip}

*Chapters also contain:*

* Solutions to exercises 
    * Exercise subsections are arranged in the same chapter --> section --> subsection as the original book
    * Chapters, sections, and subsections without exercises are usually not included
    * The beginning of sections may occassionally contain additional notes, e.g. [3.8: Position Adjustment]
* The "Appendix" sections in chapters typically contain alternative solutions to problems or additional notes/thoughts pertaining to the chapter or a related topic
    * I use the numbering scheme {chapter}.{section}.{subsection}.{problem number} to refer to exercise solutions in "Appendix" sections
* There are a few cautions with using this book[^Caution]

[^Caution]: *Cautions with book:*  
    * Beyond basic formatting clean-up, I did not substantially update the solutions from my first time going through the book. Therefore, some of the solutions and syntax may be different from how I would approach a problem now (with a couple more years coding experience).  
        * "Appendix" sections in particular received only cursory edits.  
    * Occassionally I use slightly different (or newer), methods than are shared in the book (e.g. using `mutate_at()`, `mutate_if()`, `mutate_all()` and not just `mutate()`), this is mostly confined to "Appendix" sections.  
    * Some methods in functions may be (or may become) deprecated, e.g. using `fun()` within `mutate_at()` rather than `~`.  
    * The chapter and exercise numbers are hard-coded, so if R4DS exercise order changes, the exercise solutions will no longer correspond perfectly with the R4DS source.  
    * Formatting is not always consistent between chapters, e.g. the first 14 chapters italicize or bold questions, whereas later chapters do not.  
        * Notes containing functions are usually highlighted solely with backticks, e.g. `foo`, though occassionally also have parentheses, e.g. `foo()` -- there is no logic to these differences.  
        * More formatting differences can be seen if inspecting the specific .Rmd files for each chapter.  

## Acknowledgements

*Thank you:*

* [Garrett Grolemund](https://twitter.com/StatGarrett) and [Hadley Wickham](https://twitter.com/hadleywickham) for writing a phenomenal book!
* The various [tidyverse](https://www.tidyverse.org/) and [RStudio](https://www.rstudio.com/) developers for producing outstanding packages, products, as well as resources for learning
* [R for Data Science Online Learning Community](https://www.rfordatasci.com/) and [#rstats](https://twitter.com/hashtag/rstats?src=hash&lang=en) communities for creating inspiring, safe places to post ideas, ask questions, and grow your R skills
* Stephen Kimel, who has co-organized a data science study group with me and also provided feedback on my R4DS solutions. In many cases I changed my solution to an exercise to a method that mirrored his approach.

## License

This work is licensed under a <a rel="license" href="https://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
