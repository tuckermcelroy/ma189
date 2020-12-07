---
title: "Writing Data Analysis Reports"
author: "Tucker McElroy"
date: "12/7/2020"
output: 
  html_document:
    keep_md: true
---




A data analysis report summarizes the findings of a data set's analysis.  This can be written as a static document (e.g., Markdown, Pdf, Html) or an interactive document (e.g., R Markdown Notebook).  The structure includes introduction, body, conclusion, and appendix.
 
## Audience
The report is accessible to multiple audiences, and allows each class of reader to find topics 
at their own level of detail.

### *Client or Collaborator*
They read the introduction and conclusion, and then skim body.  Organize the report around a proposed discussion with the client or collaborator.  Provide the main evidence for your conclusions with graphs and tables, placed in the body.  Leave details to the appendix.
  
### *Executive*
They will skim the introduction and conclusion.  Leave signposts (such as subsection titles) in the report to allow them zoom in and zoom out.

### *Technical Supervisor*
They read the body and appendix to examine the work's quality.  Are the methods defensible and relevant?  Have you checked assumptions?  Add text to the body and appendix so that the supervisor can understand the details of your work.

## Writing Style
Focus on content, and avoid distractions.

1. Avoid extra sentences, or formal prose, or idioms and slang.
2. Do a grammar and spell check.
3. Keep the context of data analysis appropriate for your audience.
4. Avoid details that are not needed to demonstrate your conclusions.
  
## General Structure 

1. **Introduction.** Give a summary of the study and the data, as well as the context.  Discuss the chief questions your data analysis answers.  Optionally, provide a brief outline of the report.
2. **Body.** The body can be organized by dividing into subsections, with titles such as *Data*, *Methods*, *Analysis*, and *Results*.  The *Data* section gives a proper data citation (source with url, complete title, time stamp of download) and discusses variables, time, provenance, etc.  Possibly some summary statistics or exploratory analysis (a first plot) are placed here.  Sometimes *Methods* is replaced by *Models*, and this is where you would discuss in general terms (maybe a few equations) the types of models being entertained.  *Analysis* describes what types of data analyses have been applied, and *Results* summarizes the output of those analyses.  Limit the number of tables and figures to what's really necessary to convey the chief findings.  How many tables would you want to look at?
3. **Conclusion or Discussion.**  A conclusion reprises the questions raised in the introduction, and summarizes the main findings and answers.  A discussion goes deeper into the outcomes of the analyses, explaining their repercussions to the investigation.  You can also suggest possible future questions and further work.  It is good to mention limitations of your methods, to temper conclusions accordingly. 
4. **Appendix.** All material that is too technical or bulky for the report's body goes here. This includes things such as technical descriptions of mathematical or statistical procedures; supporting tables and figures beyond the few placed in the body; computer code not already embedded in the body.  This material should be annotated: figures and tables have captions, and code is internally documented (with comment lines).
  
## Using R Markdown

R Markdown can be used to generate data analysis reports.  One can open a template file in the RStudio IDE, and the student can learn by imitation (for example, from this document). The R Markdown file can be used to generat html, pdf, or plain Markdown.  

### Markdown Versus R Markdown
Markdown is a language for quickly generating documents in the format of html, pdf, etc. Suppose you want to embed a graph or the result of a statistical calculation.  R Markdown allows you to do this.  You insert R *code chunks* into the R Markdown document.  When you *knit* in the IDE, the R code chunks are evaluated, and any output of those calculations are incorporated into your html, pdf, etc.  Nice, right?

### R Markdown Notebooks
While R Markdown is static, a R Markdown Notebook is dynamic. This means you can click on R code chunks in the notebook file, or modify the code, and the output document (html, pdf, etc.) is automatically updated. Suppose you and your collaborators want to examine a portion of the report, and modify code to see how the results change, but don't want to knit the entire document anew - then use a R Markdown Notebook.
