RECALL Questions:
0. Get the data from SGD.
```bash
wget http://data.biostarhandbook.com/data/SGD_features.tab
```

1. How to count the lines, words, and characters?
2. How to find information on gene YAL060W?
3. How can we tell how many lines DO NOT match 'Dubious'?
4. How do I store the results in a new file?
5. ORF-for protein-coding genes. How to select/view only the column of the feature ORF (column 2, include 3,4)?
6. How many lines of the protein-coding genes are non-Dubious?
7. Create a file containing the types column only.
8. How to count the unique features, and then sort from highest to lowest?
9. Alternative command to execute #9 (better formatting)?
***

0. Get the data from SGD.
```bash
wget http://data.biostarhandbook.com/data/SGD_features.tab
```
1. How to count the lines, words, and characters?
```bash
$ wc SGD_features.tab 
  16454  425719 3264490 SGD_features.tab
  
$ cat SGD_features.tab | wc 
  16454  425719 3264490
```
2. How to find information on gene YAL060W?
```bash
$ cat SGD_features.tab | grep YAL060W
S000000056	ORF	Verified	YAL060W	BDH1	(R,R)-butanediol dehydrogenase|BDH	chromosome 1		1	35155	36303	W		2011-02-03	1996-07-31|2011-02-03	NAD-dependent (R,R)-butanediol dehydrogenase; catalyzes oxidation of (R,R)-2,3-butanediol to (3R)-acetoin, oxidation of meso-butanediol to (3S)-acetoin, and reduction of acetoin; enhances use of 2,3-butanediol as an aerobic carbon source
S000036089	CDS					YAL060W		1	35155	36303	W		2011-02-03	1996-07-31|2011-02-03	
```
3. How can we tell how many lines DO NOT match 'Dubious'?
```bash
$ cat SGD_features.tab | grep -v Dubious | wc -l
15737
```
4. How do I store the results of the nonDubious features in a new file?
```bash
$ cat SGD_features.tab | grep -v Dubious > nonDubious.tab
$ cat nonDubious.tab | head
S000031098	CDS					YAL069W		1	335	649	W1996-07-31	1996-07-31	
S000031372	CDS					YAL068W-A		1	538	792	W		2003-07-29	2003-07-29	
S000121252	ARS		ARS102		ARSI-1	chromosome 1		1	707	776			2014-11-18	2014-11-18|2007-03-07	Autonomously Replicating Sequence
S000028862	telomere		TEL01L			chromosome 1		1	801	1	C	-64	2003-09-09	2003-09-09	Telomeric region on the left arm of Chromosome I; composed of an X element core sequence, X element combinatorial repeats, and a short terminal stretch of telomeric repeats
S000028864	telomeric_repeat					TEL01L		1	62	1	C		2003-09-09	2003-09-09	Terminal telomeric repeats on the left arm of Chromosome I
```
5. ORF-for protein-coding genes. How to select/view only the column of the feature ORF (column 2, include 3,4)?
```bash
$ cat SGD_features.tab | grep ORF | cut -f 2,3,4 | head
ORF	Dubious	YAL069W
ORF	Dubious	YAL068W-A
X_element		
ORF	Verified	YAL068C
ORF	Uncharacterized	YAL067W-A
ORF	Verified	YAL067C
ORF	Dubious	YAL066W
ORF	Uncharacterized	YAL065C
ORF	Uncharacterized	YAL064W-B
ORF	Uncharacterized	YAL064C-A
```
6. How many lines of the protein-coding genes are non-Dubious?
```bash
$ cat SGD_features.tab | grep ORF | cut -f 2,3,4 | grep -v Dubious | wc -l
5933
```
7. Create a file containing the types column only.
```bash
$ cat SGD_features.tab | cut -f 2 > types.tab
$ head types.tab
ORF
CDS
ORF
CDS
ARS
telomere
telomeric_repeat
X_element
X_element_combinatorial_repeat
ORF
```
8. How to count the unique features, and then sort from highest to lowest?
```bash
$ cat types.tab | sort | uniq -c | sort -rn | head
   7074 CDS
   6604 ORF
    484 noncoding_exon
    383 long_terminal_repeat
    377 intron
    352 ARS
    299 tRNA_gene
    196 ARS_consensus_sequence
     91 transposable_element_gene
     77 snoRNA_gene
```
9. Alternative command to execute #9(better formatting)?
```bash
$ cat types.tab | sort-uniq-count-rank | head
7074	CDS
6604	ORF
484	noncoding_exon
383	long_terminal_repeat
377	intron
352	ARS
299	tRNA_gene
196	ARS_consensus_sequence
91	transposable_element_gene
77	snoRNA_gene
```
