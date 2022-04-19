# Week 7

## Assignment

In the same dataset of ATAC on chr19, plot the profile of insertions (i.e. 'cuts') for the motifs of a different transcription factor, for example the glucocorticoid receptor (search "GCR").

Since most factors bind only a small minority of their motifs, you'll most likely have to restrict the motif instances to those that are in accessible regions, e.g. 
```r
motifs_GCR <- findMotifInstances(chr19, motif_GCR)
accessible_regions <- callPeaks("atac.chr19.bam")
seqlevelsStyle(peaks) <- "Ensembl"
accessible_motifs <- motifs_GCR[overlapsAny(motifs_GCR, accessible_regions)]
```

### Expected form of the answer:

A figures containing the heatmaps of the two signals around the motifs

Don't forget to render your markdown and push it as `assignment.html` !

