Reproducibility
================
Valerie Han
2023-02-23

![Frontmatter check](../../actions/workflows/check-yaml.yaml/badge.svg)

## Prompt:

In May 2015 Science retracted - without consent of the lead author - a
paper on how canvassers can sway people’s opinions about gay marriage,
see also:
<http://www.sciencemag.org/news/2015/05/science-retracts-gay-marriage-paper-without-agreement-lead-author-lacour>
The Science Editor-in-Chief cited as reasons for the retraction that the
original survey data was not made available for independent reproduction
of results, that survey incentives were misrepresented and that
statements made about sponsorships turned out to be incorrect.<br> The
investigation resulting in the retraction was triggered by two Berkeley
grad students who attempted to replicate the study and discovered that
the data must have been faked.

[FiveThirtyEight](https://fivethirtyeight.com/features/how-two-grad-students-uncovered-michael-lacour-fraud-and-a-way-to-change-opinions-on-transgender-rights/)
has published an article with more details on the two Berkeley students’
work.

Malicious changes to the data such as in the LaCour case are hard to
prevent, but more rigorous checks should be built into the scientific
publishing system. All too often papers have to be retracted for
unintended reasons. [Retraction Watch](https://retractionwatch.com/) is
a data base that keeps track of retracted papers (see the related
[Science
magazine](https://www.sciencemag.org/news/2018/10/what-massive-database-retracted-papers-reveals-about-science-publishing-s-death-penalty)
publication).

Read the paper [Ten Simple Rules for Reproducible Computational
Research](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003285)
by Sandve et al.

Write a blog post addressing the questions:

1.  Pick one of the papers from Retraction Watch that were retracted
    because of errors in the paper (you might want to pick a paper from
    the set of featured papers, because there are usually more details
    available). Describe what went wrong. Would any of the rules by
    Sandve et al. have helped in this situation?

I chose to read this paper:

Liwen Hu, Shunsuke Saito, Lingyu Wei, Koki Nagano, Jaewoo Seo, Jens
Fursund, Iman Sadeghi, Carrie Sun, Yen-Chun Chen, and Hao Li. 2017.
Avatar digitization from a single image for real-time rendering. ACM
Trans. Graph. 36, 6, Article 195 (December 2017), 14 pages.
<https://doi.org/10.1145/3130800.31310887>.

This paper is one of two papers coauthored by Hao Li that will be
retracted soon due to the publishers discovering falsification of data
in the papers. Given that it appears that the authors purposely
falsified the results, I think the main way to prevent a situation like
this happening again would more details on the process so that someone
reading the article could reproduce the results with different images.
The most pertinent rules would be 1, 2, and 10. However, I’m not sure if
requiring rule 10 would be possible in such a situation since I don’t
know if you could still make a company based on the methods in the paper
if you share all the code.

2.  After reading the paper by Sandve et al. describe which rule you are
    most likely to follow and why, and which rule you find the hardest
    to follow and will likely not (be able to) follow in your future
    projects.

Rule 2 (avoiding manual data manipulation steps) is the rules I am most
likely to follow since `tidyverse` makes it really easy to use code to
manipulate/explore data. I think in general the thing that makes the
rules hard to follow strictly is recording so much information. In
particular, Rule 1 (keeping track of how every result was produced) is
probably the most difficult, though I can see why it would make my
future self’s life so much easier.

## Submission

1.  Push your changes to your repository.

2.  You are ready to call it good, once all your github actions pass
    without an error. You can check on that by selecting ‘Actions’ on
    the menu and ensure that the last item has a green checkmark. The
    action for this repository checks the yaml of your contribution for
    the existence of the author name, a title, date and categories.
    Don’t forget the space after the colon! Once the action passes, the
    badge along the top will also change its color accordingly. As of
    right now, the status for the YAML front matter is:

![Frontmatter check](../../actions/workflows/check-yaml.yaml/badge.svg)

    ---
    author: "Your Name"
    title: "Specify your title"
    date: "2023-02-23"
    categories: "Ethics and Reproducibility..."
    ---