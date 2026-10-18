# MiniProject Use Qualitative Analysis

## Background 

In MiniProject2, you analyzed ten projects, producing time-series
plots, summaries, and reflections. In this final phase, you will
move from analysis to validation. Each student will now review ten projects from their teammate (see teammates in the table below)
to ensure that the interpretations and classifications are accurate
and consistent across the class (key step in any qualitative
analysis). This step focuses on learning how to improve data
quality, resolve differences in interpretation, and generate richer
qualitative understanding of a dataset.

1. Please go over [Qualitative Analysis Slides](./QualitativeAnalysis.pdf) in Lectures repository
2. Please inspect the [Coding Guide used for MiniProject2](./CodingGuide.csv)

## Part 1 due Oct 13
### Independent Review

1. Access the MiniProject2 repository of your teammate from the table below: you will be reviewing the results they produced.

2. For each of the fields listed below, record your own judgment in YOURnetid_validation_log.csv, creating a row for each project-field combination for the following fields. Refer to [netid_validation_log_example.csv](./netid_validation_log_example.csv) for the proper formatting
    - HasRecovered
    - WhyRecovered
    - ActivityPattern
    - Currentstatus
    - RecentThemes
3. To facilitate discussion in Part 2, order rows so that for each question (field) all 10 projects are listed then rows for the next field are started.
4. YOURnetid_validation_log.csv will have the following columns:

|WOCProjectID|ProjectOwnerNetID|ValidatorNetID|Field(one out of five listed above)|AuthorValue|ValidatorValue|PreDiscussAgreementstatus(Yes/No)|AdjudicatedValue|KeyEvidence|Comments|
|-|-|-|-|-|-|-|-|-|-|

5. In this step, populate just ProjectOwnerNetID; ValidatorNetID;
Field; AuthorValue; ValidatorValue; PreDiscussAgreementstatus(Yes/No); and KeyEvidence;

## Part 2 done on Oct 13 in class
### Discuss and Resolve

Time at the end of class on Oct 13 will be used to facilitate discussion of
discrepancies between your MiniProject2 and your teammate's validations of MiniProject2 from Part 1. If you cannot attend class Oct 13th, you can choose to hold discussions any time before MiniProject3 Deadline. Between you and your teammate, there are 100 total records to review(five fields, and 10 projeacts for each student) . For this part, we only concern ourselves with the subset of records which disagree.

1. Each student commits their teammate's YOURnetid_validation_log.csv into their repository.
1. For every disagreement, hold an evidence-based conversation to decide an Adjudicated Value and enter it in the YOURnetid_validation_log.csv spreadsheet under the AdjudicatedValue column.
1. Create a YOURnetid_disagreement_examples.md and record at least three distinct examples of disagreements and their resolutions (complete with project id, and parties of discussion).
1. Create YOURnet_id_disagreement_resolution and record all disagreements (by selecting the relevant subset of rows from YOURnetid_validation_log.csv) with columns: 

|WOCProjectID|ProjectOwnerNetID|ValidatorNetID|Field|AuthorValue|ValidatorValue|AdjudicatedValue|ResolutionType(AuthorKept ValidatorKept/Compromise)|PostDiscussAgreementstatus(Yes/No)|KeyEvidence|Comments|
|-|-|-|-|-|-|-|-|-|-|-|

Fill in all columns with information gained from your discussions.

## Part 3 due Oct 19th
### Update and Synthesis

1. Create YOURnetid_agreement_stats.csv and summarize the level of agreement across all 5 validated fields with the following columns:

|Field|PercentAgree_Pre|PercentAgree_Post|CohenKappa_Pre|CohenKappa_Post|NumDisagreements|NumResolved|Notes|
|-|-|-|-|-|-|-|-|

2. Each row in this CSV corresponds to one validated field. See How to compute column values below.
2. Create YOURnetid_validation_reflection.md and write a few paragraphs of validation reflection, connecting adjudicated labels to patterns seen across projects; which signals precede long gaps, what triggers recovery, and when gaps don’t mean project death. Highlight recurring interpretation pitfalls and how they were resolved.
   

## Submission Checklist

 - YOURnetid_validation_log.csv
 - YOURnetid_disagreement.md
 - YOURnet_id_disagreement_resolution.csv
 - YOURnetid_agreement_stats.csv
 - YOURnetid_validation_reflection.md


### Calculations for YOURnetid_agreement_stats.csv:

PercentAgree_Pre = (Number of “Agree” before discussion ÷ Total comparisons) × 100

PercentAgree_Post = (Number of “Agree” after discussion ÷ Total comparisons) × 100

Example: If 15 out of 20 projects matched before discussion → 15/20 × 100 = 75%
If 19 out of 20 matched after discussion → 19/20 × 100 = 95%
Round all percentages to one decimal place.

Cohen’s κ (Kappa): Report Cohen’s κ only for categorical fields (ActivityPattern, CurrentStatus, HasRecovered) to measure inter-rater reliability. Example: if κ = 0.85 post-discussion, it indicates strong agreement. For all non-categorical fields (BeforeThemes, AfterThemes, HypothesizedReason, RecentThemes, Notes), enter NA for both CohenKappa_Pre and CohenKappa_Post.

Notes Column:  Summarize any relevant patterns or challenges (e.g., “Terminology mismatches,” “Improved clarity after examples”).

# Partners for MiniProject3 by NetID

If you do not see your netID listed below or your partner is unreachable/dropped the class, please email me: jhammer3@vols.utk.edu

You can map names/githubIDs for each NetID in [netids.md](./netID.md).


|peer A| peer B|
|-|-|
|jtyuill|hsaleh5|
|asaucer|bslessma|
|jharves1|tcartier|
|melawady|mjohn326|
|bjy819|hawad|
|jpark127|kha5|
|pvickery|cboddick|
|oyoungbl|aberard|
|dkim68|eabbott9|
|ddemarco|econstan|
|sydlwils|jzr266|
|lsantucc|pstorch1|
|jbronyah|kyandall|
|lwang111|ccoughl3|
|wch356|jvijayak|
|ltipto11|hneel|
|wknepp|aalkafou|
|gelkhoda|sbombry1|
|arother1|cfinley6|
|smaciasa|cwolver1|
|pshu|gkhot|
|cgoering|dmengeli|
|spate198|mmariaru|
|kbc177|asangiul|
|jmill291|bdowlin2|
|hnaicker|gwright30|
|astubbin|pmarino|
|aamphone|tgarrio1|
|ggood3|smazunda|
|emolder|rkabarwa|
|jmurph91|tlopez7|
|hcrettol|jbell96|
|ksaravan|dbritto3|
|smurph61|spastor|
|amart170|ttb615|
|bxy539|afink12|
|kbissonn|hvo5|
|ccolli78|bnoyes|
|dlong37|dpate172|
|cdamron3|ncash3|
|cliddel2|pvathana|
