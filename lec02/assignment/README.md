#Application of Lecture + Self Discovery
Organism Selected: salmo_salar

```bash
$ wget https://ftp.ensembl.org/pub/current_gff3/salmo_salar/Salmo_salar.Ssal_v3.1.115.gff3.gz
```

1. Tell us a bit about the organism.
<div style="word-break: break-word;">
  Salmo salar, or the Atlantic salmon, is a large, anadromous fish native to the 
  northern Atlantic Ocean and its connecting rivers. It is known for its 
  impressive migrations between freshwater and saltwater environments.Salmo salar, or the Atlantic salmon, 
  is a large, anadromous fish native to the northern Atlantic Ocean and its connecting rivers. 
  Key for its unique ability to survive spawning and return to the sea multiple times, 
  it is the most common species in global aquaculture, particularly in Norway, Chile, and Canada. 
  While it remains a vital source of omega-3 fatty acids, wild populations are currently 
  listed as Near Threatened due to overfishing and habitat loss.<br><br>

  Alias=HG993288 \
  https://www.ebi.ac.uk/ena/browser/view/HG993284
<table>
  <thead>
    <tr>
      <th>Property</th>
      <th>Value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Organism</strong></td>
      <td>Salmo salar (Atlantic salmon)</td>
    </tr>
    <tr>
      <td><strong>Accession</strong></td>
      <td>HG993284</td>
    </tr>
    <tr>
      <td><strong>Mol Type</strong></td>
      <td>genomic DNA</td>
    </tr>
    <tr>
      <td><strong>Topology</strong></td>
      <td>linear</td>
    </tr>
    <tr>
      <td><strong>Base Count</strong></td>
      <td>54,385,492</td>
    </tr>
    <tr>
      <td><strong>Dataclass</strong></td>
      <td>CON</td>
    </tr>
    <tr>
      <td><strong>Tax Division</strong></td>
      <td>VRT</td>
    </tr>
    <tr>
      <td><strong>Assembly Accession</strong></td>
      <td>GCA_905237065</td>
    </tr>
    <tr>
      <td><strong>Chromosome</strong></td>
      <td>ssa25</td>
    </tr>
    <tr>
      <td><strong>Md5 Checksum</strong></td>
      <td>1d3cd37ba846c3c8e7a5e38e69e5e9cc</td>
    </tr>
  </tbody>
</table>

<br>

https://www.ncbi.nlm.nih.gov/datasets/genome/GCA_931346935.2/

<table style="width: 100%; border-collapse: collapse; font-family: sans-serif; border: 1px solid #ddd;">
  <thead>
    <tr style="background-color: #f2f2f2; text-align: left;">
      <th style="padding: 12px; border-bottom: 2px solid #ddd;">Metric</th>
      <th style="padding: 12px; border-bottom: 2px solid #ddd;">Value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">Genome Size</td>
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">2.6 Gb</td>
    </tr>
    <tr style="background-color: #f9f9f9;">
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">Total Ungapped Length</td>
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">2.6 Gb</td>
    </tr>
    <tr>
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">Gaps Between Scaffolds</td>
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">447</td>
    </tr>
    <tr style="background-color: #f9f9f9;">
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">Number of Chromosomes</td>
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">29</td>
    </tr>
    <tr>
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">Number of Scaffolds</td>
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">4,042</td>
    </tr>
    <tr style="background-color: #f9f9f9;">
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">Scaffold N50</td>
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">19.2 Mb</td>
    </tr>
    <tr>
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">Scaffold L50</td>
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">39</td>
    </tr>
    <tr style="background-color: #f9f9f9;">
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">Number of Contigs</td>
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">4,067</td>
    </tr>
    <tr>
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">Contig N50</td>
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">19.2 Mb</td>
    </tr>
    <tr style="background-color: #f9f9f9;">
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">Contig L50</td>
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">39</td>
    </tr>
    <tr>
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">GC Percent</td>
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">43.5%</td>
    </tr>
    <tr style="background-color: #f9f9f9;">
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">Genome Coverage</td>
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">27x</td>
    </tr>
    <tr>
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">Assembly Level</td>
      <td style="padding: 10px; border-bottom: 1px solid #ddd;">Chromosome</td>
    </tr>
  </tbody>
</table>

</div>

<br>

2. How many sequence regions (chromosomes) does the file contain? Does that match with the expectation for this organism?
<br>There are 29 sequence regions. Yes, it matches the 29 haploid chromosomes as it is published in NCBI Genome assembly Ssal_ALTA.
```bash
$ zcat Salmo_salar.Ssal_v3.1.115.gff3.1.gz | grep -v "#" | grep -w "region"| grep 'ssa'| wc -l && \ 
> zcat Salmo_salar.Ssal_v3.1.115.gff3.1.gz | grep -v "#" | grep -w "region"| grep 'ssa'| head -3
29
1	Ssal_v3.1	region	1	174498729	.	.	.	ID=region:1;Alias=HG993260.1,ssa01
10	Ssal_v3.1	region	1	125877811	.	.	.	ID=region:10;Alias=HG993269.1,ssa10
11	Ssal_v3.1	region	1	111868677	.	.	.	ID=region:11;Alias=HG993270.2,ssa11
```

3. How many features does the file contain?
<br>It contains 4,716,412 features.
```bash
$ zcat Salmo_salar.Ssal_v3.1.115.gff3.1.gz | grep -v "#" | cut -f 3 | head                          
region
biological_region
biological_region
biological_region
biological_region
biological_region
biological_region
biological_region
gene
mRNA

$ zcat Salmo_salar.Ssal_v3.1.115.gff3.1.gz | grep -v "#" | cut -f 3 | wc -l
4716412
```
4. How many genes are listed for this organism?
<br>It contains 47,205 genes.
```bash
$ features=$(zcat Salmo_salar.Ssal_v3.1.115.gff3.1.gz | grep -v "#" | cut -f 3 | sort-uniq-count-rank); echo "$features"
2107386	exon
1853224	CDS
197091	five_prime_UTR
175342	three_prime_UTR
146010	mRNA
125760	biological_region
47205	gene
28710	lnc_RNA
21576	ncRNA_gene
5197	rRNA
4011	region
2059	snRNA
901	snoRNA
608	pseudogene
608	pseudogenic_transcript
480	miRNA
123	V_gene_segment
56	transcript
34	D_gene_segment
24	scRNA
5	J_gene_segment
2	Y_RNA

$ zcat Salmo_salar.Ssal_v3.1.115.gff3.1.gz | grep -v "#" | cut -f 3 | sort-uniq-count-rank | grep -w 'gene'
47205	gene
```
5. Is there a feature type that you may have not heard about before? What is the feature and how is it defined? (If there is no such feature, pick a common feature.)
<br>
lnc_RNA, ncRNA_gene, snRNA, snoRNA, pseudogene, pseudogenic_transcript, V_gene_segment, D_gene_segment, J_gene_segment, transcript, Y_RNA

As such, here's the definition of each:
<table border="1" style="border-collapse: collapse; width: 100%; font-family: Arial, sans-serif;">
  <thead>
    <tr style="background-color: #f2f2f2;">
      <th style="padding: 10px; text-align: left;">Feature Type</th>
      <th style="padding: 10px; text-align: left;">Concise Definition</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="padding: 8px;"><strong>ncRNA_gene</strong></td>
      <td>A gene that functions as RNA directly and is <strong>not</strong> translated into a protein.</td>
    </tr>
    <tr>
      <td style="padding: 8px;"><strong>lnc_RNA</strong></td>
      <td>"Long" non-coding RNA (>200 nt) that regulates how other genes are turned on or off.</td>
    </tr>
    <tr>
      <td style="padding: 8px;"><strong>snRNA</strong></td>
      <td>"Small Nuclear" RNA; the machinery used to <strong>splice</strong> introns out of mRNA.</td>
    </tr>
    <tr>
      <td style="padding: 8px;"><strong>snoRNA</strong></td>
      <td>"Small Nucleolar" RNA; guides that help chemically modify other RNAs (like rRNA).</td>
    </tr>
    <tr>
      <td style="padding: 8px;"><strong>Y_RNA</strong></td>
      <td>Small RNAs involved in DNA replication and maintaining RNA stability.</td>
    </tr>
    <tr>
      <td style="padding: 8px;"><strong>pseudogene</strong></td>
      <td>A "genomic fossil"; a sequence that looks like a gene but is broken by mutations.</td>
    </tr>
    <tr>
      <td style="padding: 8px;"><strong>pseudogenic_transcript</strong></td>
      <td>An RNA molecule produced by a pseudogene (usually non-functional).</td>
    </tr>
    <tr>
      <td style="padding: 8px;"><strong>V, D, J_gene_segment</strong></td>
      <td>"Lego-like" DNA fragments used by the immune system to build custom <strong>antibodies</strong>.</td>
    </tr>
    <tr>
      <td style="padding: 8px;"><strong>transcript</strong></td>
      <td>A general term for any RNA molecule produced by a gene before it is specifically classified.</td>
    </tr>
  </tbody>
</table>

6. What are the top-ten most annotated feature types (column 3) across the genome?
The top-ten are the following:<br>
<table border="1" style="border-collapse: collapse; width: 300px; font-family: Arial, sans-serif;">
  <thead>
    <tr style="background-color: #f2f2f2;">
      <th style="padding: 8px; text-align: left;">Count</th>
      <th style="padding: 8px; text-align: left;">Feature Type</th>
    </tr>
  </thead>
  <tbody>
    <tr><td style="padding: 8px;">2,107,386</td><td style="padding: 8px;">exon</td></tr>
    <tr><td style="padding: 8px;">1,853,224</td><td style="padding: 8px;">CDS</td></tr>
    <tr><td style="padding: 8px;">197,091</td><td style="padding: 8px;">five_prime_UTR</td></tr>
    <tr><td style="padding: 8px;">175,342</td><td style="padding: 8px;">three_prime_UTR</td></tr>
    <tr><td style="padding: 8px;">146,010</td><td style="padding: 8px;">mRNA</td></tr>
    <tr><td style="padding: 8px;">125,760</td><td style="padding: 8px;">biological_region</td></tr>
    <tr><td style="padding: 8px;">47,205</td><td style="padding: 8px;">gene</td></tr>
    <tr><td style="padding: 8px;">28,710</td><td style="padding: 8px;">lnc_RNA</td></tr>
    <tr><td style="padding: 8px;">21,576</td><td style="padding: 8px;">ncRNA_gene</td></tr>
    <tr><td style="padding: 8px;">5,197</td><td style="padding: 8px;">rRNA</td></tr>
  </tbody>
</table>

7. Having analyzed this GFF file, does it seem like a complete and well-annotated organism?
8. Share any other insights you might note.
