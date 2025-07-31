# Seminar 1

This repository contains the reports and presentation for Seminar 1 from Remote Ruckus (Team 1)

**Seminar details**:
Title: ...
Time: Tuesday 1-2pm 5th August
Location: HM LT001 
Team members:
- Dwayne Mark (Dwayne) Acosta
- Mohamed Amine (Mohamed) Benaziza
- David Franz
- Ray Marange
- James Thompson

## Instructions

Insturctions copied from the website: https://ecs.wgtn.ac.nz/Courses/AIML430_2025T2/Seminar1

> - Your group will produce a summary of an assigned paper (3% group mark). You will have the option to submit your own individual summary if you face group work difficulties --- though this will greatly increase your own workload! No student has chosen this option since the course started...
> - The summary should be ~2 pages longer (no more than 4!). You are encouraged (and expected) to include your own takeaways/thoughts. It will be given to your classmates before your seminar as reading material.
> - Your group will then facilitate a seminar on your assigned paper. You will start with a short presentation (max 10 mins, 1%, individual mark) and then take turns facilitating discussion on a question asked by (preferably) your classmates or the lecturers (1%, individual mark).
> - You will have the opportunity to form your own group. Those who do not have a group by the registration deadline will be assigned one by the lecturer. 


## Contributers

The documents are in LaTeX. The summary report is called [summary.tex](summary.tex) and the presentation is called [presentation.tex](presentation.tex).

The output pdfs of these can be found in the [output](output/) directory.

The bibliography is in Bibtex format, [references.bib](references.bib).

### Building documents

I use LaTeX workshop in vscode to do my work. However if you want to just build manually you can do so as well.
Assuming you have a Tex distribution installed you can just run

```bash
latexmk -pdf summary.tex -output-directory=output
latexmk -pdf presentation.tex -output-directory=output
latexmk -c --output-directory=output
```

It will build both documents with the dependencies.

### Adding referecnes

To add referecnes add the bibtex entry directly into the references.bib file. Then you can use the usual `\cite{...}` command.

### Pushing to main

You should push to main regularly and reoslve merge conflicts immeditately. This will help us to stay as synced as possible. Whenever you make it to some 'point' be it first draft or what have you then commit and push.
