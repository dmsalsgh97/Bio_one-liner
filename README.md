# Bio_one-liner
useful one-liner command for bioinfomatics

# bam/sam to fasta
samtools view filename.bam | awk '{OFS="\t"; print ">"$1"\n"$10}' - > filename.fasta
