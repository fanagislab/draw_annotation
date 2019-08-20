Description:
After annotate genes, ncRNAs, repeats, and other elements, we should map all these resources to
the chromosome, the figures are drawn to get an integrated view.

Programs:
  map_genome.pl  (draw figures for the whole genome)
    map_chromosome.pl  (draw figure for a specified chromosome with a specified region)

Examples:
   perl ../bin/map_chromosome.pl --sequence chr1  --startpos 1000001  --endpos  2000000 --gene ../input/test_3chrs.fa.bgf.gff --genemark bgf  --gene ../input/test_3chrs.fa.genscan.gff --genemark genscan  --feature ../input/test_3chrs.fa.RepeatMasker.out.gff --featmark TE --feature ../input/test_3chrs.fa.trf.dat.gff --featmark TRF 

  make_genome_gff.pl ./9311_Chr01.fa > ./9311_Chr01.fa.gff

  perl ../bin/map_genome.pl ../input/test_3chrs.fa.gff --gene ../input/test_3chrs.fa.bgf.gff --genemark bgf --gene ../input/test_3chrs.fa.genscan.gff --genemark genscan --feature ../input/test_3chrs.fa.RepeatMasker.out.gff --featmark TE --feature ../input/test_3chrs.fa.trf.dat.gff --featmark TRF
