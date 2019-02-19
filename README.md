# Pleurozium_schreberi_annotated_genome_files

Annoatated genome of moss Pleurozium schreberi

* BILS Genome Annotation Platform team *
Fri Jun  1 14:59:20 CEST 2018
Please find here an overview about data available.

<Species_Annotation_Report.docx> file => A complete report of work/process performed.
================================

<fasta> directory => It contains data in FASTA format.
=================	<cds.fasta> file => It contains cds of annotated genes.
			<protein.fasta> file => It contains the proteins produced by the annotated genes.
	<transcripts> sub directory
	===========     <Trinity_*_.fasta> is the output of our Trinity pipeline used as inout for Maker.

<gff> directory => It contains data in gff3 format.
===============

	<gene-builds> sub directory

	===========	<species_rcX.gff> Are the “release candidate” annotation for the species. The higher release candidate corresponds to the most successful achievement.

	<lift-overs> sub directory (depending on customer demand)
	============	<referenceSpecies2studiedSpecies.gff> It is the lift-over of a reference species genome annotation (from Ensembl) on the genome under investigation.

	<ncRNA> sub directory
	=======		<ncRNA_rfam.gff> It contains annotation of non-coding element annotated using the Eucaryotes data from Rfam database.
			<*_tRNA.gff> It contains transfert RNA annotated using tRNAscan.

	<repeats> sub directory
	=======	<repeatmasker.gff> It contains repeats annotated thanks to repeatmasker.
		<repeatrunner.gff> It contains repeats annotated thanks to repeatrunner.

	<transcripts> sub directory
	===========       <Cufflinks_*.gff> contains output of our Cufflinks pipeline used as input for Maker. (Depending of RNAseq data types, and the most appropriate Transcriptome assembly method chosen.)
			  <Trinity_*.gff> is the gff output created by Maker using the Trinity_*_.fasta file as input. (Depending of RNAseq data types, and the most appropriate Transcriptome assembly method chosen.)
			  <*> Depending of RNAseq data types, and the most appropriate Transcriptome assembly method chosen.

<metadata> directory
==========	<go.txt> Tab-delimited format file (2 rows) containing GO terms of functions retrieved for each transcript.
		<pfam.txt> Tab-delimited format file (2 rows) containing pram terms of functions retrieved for each transcript.
		<interpro.txt> Tab-delimited format file (2 rows) containing interpro terms of functions retrieved for each transcript.

<summary> directory
=========	<coding_gene.txt> General information about annotated coding genes
		<tRNA.txt> General information about annotated tRNA
