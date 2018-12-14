# frmt
Data Formats
Same Data, Different Formatsclick to collapse

A number of different data presentation formats have been used to represent genetic strings. The history of file formats presents its own kind of evolution: some formats have died out, being replaced by more successful ones. Three file formats are currently the most popular:

FASTA (.fas, .fasta): used by practically all modern software and databases, including ClustalX, Paup, HyPhy, Rdp, and Dambe.
NEXUS (.nex, .nexus, .nxs): used by Paup, MrBayes, FigTree, and SplitsTree.
PHYLIP, or "Phylogeny Inference Package" (.phy): used by Phylip, Tree-Puzzle, PhyML, and a number of databases.
A simple reference on file formats can be found here.

In this problem, we will familarize ourselves with FASTA. We will save the other two formats for later problems.

In FASTA format, a string is introduced by a line that begins with '>', followed by some information labeling the string. Subsequent lines contain the string itself; the next line beginning with '>' indicates that the current string is complete and begins the label of the next string in the file.

GenBank hosts its own file format for storing genome data, containing a large amount of information about each interval of DNA. The GenBank file describes the interval's source, taxonomic position, authors, and features (see Figure 1).

A sample GenBank entry can be found here. You may export an entry to a variety of file formats by selecting the appropriate file format under the Send To: dropdown menu at the top of the page.

Problem
GenBank can be accessed here (https://www.ncbi.nlm.nih.gov/genbank/). A detailed description of the GenBank format can be found here. A tool, from the SMS 2 package, for converting GenBank to FASTA can be found here.

Given: A collection of n (n≤10) GenBank entry IDs.

Return: The shortest of the strings associated with the IDs in FASTA format.
