

\# Day 12 — Galaxy QC → Trim → Assembly → QUAST

\#\# Sample  
\- sampleID: wt  
\- raw data: (where it came from / dataset name)WT\_R1.fastq.gz  
WT\_R2.fastq.gz

\#\# Tools (Galaxy / usegalaxy.org)  
\- FastQC: Galaxy Version 0.74+galaxy1  
\- fastp: Galaxy Version 1.1.0+galaxy0  
\- SPAdes: Galaxy Version 4.2.0+galaxy0  
\- QUAST: Galaxy Version 5.3.0+galaxy1

\#\# Steps  
1\. FastQC on raw reads → saved report as: forward(reverse)\_fastqc.html  
2\. fastp trimming (default settings) → saved report as: wt\_fastpreport.html  
3\. FastQC on trimmed reads → saved report as: forward(reverse)trim\_fastqc.html  
4\. SPAdes assembly on trimmed reads → saved contigs as: wt\_spades\_contigs.fasta  
5\. QUAST evaluation on contigs → saved report as: wt\_quastreport.pdf

\#\# Notes / interpretation  
\- ( – For the forward data nothing really changed besides the read length– overall there wasn't a noticeable change – Removing low quality bases helps decrease errors down stream).  
\- (There were 79 contigs so the genome was not a single continuous sequence it was fragmented – N50 indicates large cover portions of the genome – L50 indicates moderate assembly quality)

