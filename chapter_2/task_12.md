# Task 12 - SNPs and Indels

*The following 3 tasks are open-ended. Please take your time with these. Don't forget though, there's more adventures to be had!*

## Alignment Display Format
Visit  the BROAD's website [here](http://www.broadinstitute.org/software/igv/AlignmentData) :mag: and have a brief read of the format.

## Manually Identify a Region Without any Reads Mapping
These regions can be quite difficult to find even with a very small genome. Zoom out as far as you can and still see the reads. Use the coverage plot from QualiMap to try to find it. Are there any genes associated with this region?

Because of the way IGV handles BAM files, it will not display coverage information if you zoom out too far. To be able to see this coverage information across the entire genome, regardless of how far you are zoomed out, you’ll need to create a 'TDF file' which contains a coverage information across windows of X number of bases across the genome.

You can do this within IGV:

> Select Tools->Run igvtools

[IMAGE]

> Load the BAM alignment file in the Input field and click Run

[IMAGE]

Once completed, close the igvtools window and then you can load this TDF file:

> Select File -> Load from file…

[IMAGE]

You should then see the extra coverage track which remains visible even after you zoom out. 