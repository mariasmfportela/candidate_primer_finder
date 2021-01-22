# Candidate Primer Finder
Basic script to identify primer candidates from a gene sequence.

Use: modify the string variables "exon1" and "exon2" with the FASTA sequence for your gene of interest, in uppercase and with no whitespaces. The forward primer candidates are chosen in exon 1 and the reverse primer candidates are chosen in exon 2. Run the script with your favourite Python service. It will print out candidate primer sequences in the direction 5'-3'. 

All primer candidates identified are 20bp long, with 50-55% GC content and with a GC clamp at the 3' end.
You should still verify the candidates are suitable primers for your experiment as this script doesn't check for self-complementarity or hairpin formation, for example. You should take the reverse complement of the reverse primer candidates before use.
