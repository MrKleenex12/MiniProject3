# Validation Reflection — lwang111

I validated ten projects from ccoughl3's MiniProject2, five fields per project.
Agreement was perfect on the three categorical fields: HasRecovered,
ActivityPattern, and Currentstatus (100% agreement, Cohen's κ = 1.0 both before
and after discussion). All six disagreements were in the free-text fields:
four in WhyRecovered (60% agreement before discussion) and two in RecentThemes
(80%). We resolved all six through discussion, so post-discussion agreement
reached 100% for every field. Three disagreements were resolved in the author's
favor and three by compromise. None were resolved by keeping my value
unchanged.

The adjudicated labels show some patterns across the projects. Long gaps
usually came after a declining activity pattern. Five of the ten projects were
labeled declining, and two of them (ceedee666_opensap_python_intro and
hol137_jupyter-notebook-practice-physical-constants-ratios) never recovered.
Both are course or practice repositories, which have a natural end point, so
their gaps look like completion rather than failure. Recovery was usually
triggered by outside pressure, not new plans: a dependency bump (asteval in
numenta_nupic), a toolchain break (the Xcode 16 build failure in
cardinalkit_cardinalkit), automated code changes (deepmind_acme), or backlog
bug fixes and merges (qupath_qupath, annecori_epiestim). New feature work as a
reason for returning was rare. sem-jl_sem.jl was the clearest case.

A gap also did not always mean the project was dead, and a recovery did not
always mean it was alive. numenta_nupic and yulunzhang_rcan both counted as
"recovered" but are currently inactive. Their post-gap commits were small
maintenance or administrative changes (a dependency update, README/license
edits, Google Drive link updates). I first recorded two of these recoveries as
"Yes, but barely." That hedge is a sign that HasRecovered alone can overstate
how healthy a project is. Reading it together with Currentstatus and
ActivityPattern gives a more accurate picture. On the other hand, irregular
projects such as lfpy_lfpy and sem-jl_sem.jl had long gaps but are still
active, so for them a quiet period was a normal part of the cycle, not
abandonment.

Two interpretation pitfalls came up repeatedly. The first was **granularity**.
In WhyRecovered, I often named the most visible single commit ("Update readme
and MIT license", "Update Google Drive", "Fix conflicts"), while the author
described the underlying cause ("update asteval", "administrative changes",
"work on other parts of the project"). We resolved these by asking which
commit actually brought the project back. That kept the author's value when
the visible commit was only a side effect (numenta_nupic, sem-jl_sem.jl) and
combined the two when both were real (qupath_qupath, yulunzhang_rcan). The
second pitfall was **vocabulary drift**. In RecentThemes I used labels outside
the coding guide ("Conflicts", "Update readme"). We fixed these by mapping them
back to the guide's themes, such as Other (merges) and Bug fixes. ccoughl3's
review of my projects showed the opposite problem: we disagreed more on
ActivityPattern and Currentstatus (for example, declining vs. irregular, and
Active vs. Inactive for projects with only a few recent commits). This
suggests that shape and recency labels need explicit thresholds in the coding
guide, while the free-text fields need a fixed list of allowed values. Both
changes would cut down the number of disagreements that need discussion.
