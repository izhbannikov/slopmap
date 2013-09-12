/***********************************************Usage******************************************************************/

Paired-end Illumina:

./slopmap -1 <PE1 filename> -2 <PE1 filename> -l <Library name> -o <Output prefix> [-k <KMER_SIZE> -d <DISTANCE> -t <THRESHOLD>]


Single-end Illumina:

./slopmap -U <SE filename> -l <Library name> -o <Output prefix> [-k <KMER_SIZE> -d <DISTANCE> -t <THRESHOLD>]


Roche 454:

./slopmap -454 <454 filename> -l <Library name> -o <Output prefix> [-k <KMER_SIZE> -d <DISTANCE> -t <THRESHOLD>]


Default parameters:

-k <KMER_SIZE> 11

-d <DISTANCE> 5 (distance between two consecutive k-mers)

-t <THRESHOLD> 0.75


/***********************************************Examples******************************************************************/

-Paired-end Illumina:

./slopmap -1 <SlopMap HOME>/test_data/R1.fastq.gz -2 <SlopMap HOME>/test_data/R2.fastq.gz -o test -l <SlopMap HOME>/test_data/vectors.fasta -t 0.9


-Single-end Illumina:

./slopmap -U <SlopMap HOME>/test_data/R1.fastq.gz -o test -l <SlopMap HOME>/test_data/vectors.fasta -t 0.83 -d 3


-Roche 454:

./slopmap -454 <SlopMap HOME>/test_data/SmallTest.sff -o test -l <SlopMap HOME>/test_data/vectors.fasta -t 0.56 -k 14



