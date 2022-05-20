# Week 11

## Assignment

- Choose a transcription factor (e.g. p300), and obtain peaks from ENCODE
  - make sure it’s the same cell line, i.e. A549, or that Hi-C interactions are available for your cellular context!
- Isolate the peaks that are:
  - Between 2.5kb and 10kb from a TSS
  - More than 10kb from a TSS
- For each set of peaks, identify those that are in contact with a TSS using long-range interactions from ENCODE
- For each set, **what proportion of the interactions are with the nearest gene?**
- Hints:
  - you can use the `annotateRegions` function, as we did in week 4, to get the gene nearest to each peak
  - beware not to count, when calculating proportions, peaks that don’t have interactions with any TSS!
- Expected for of the answer:
  - "Of the genes that are between 2.5 and 10kb from the nearest TSS, XX % form an interaction with that nearest gene. Of the genes that are more than 10kb away from the nearest TSS, XX % form an interaction with that nearest gene."

