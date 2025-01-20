# Variant_Calling
Example command for varinat calling 

gatk Mutect2 \
  --sequence-dictionary $REFERENCE_DICTIONARY \
  --reference $REFERENCE_SEQUENCE \
  --input $NORMAL_BAM_FILE \
  --normal-sample $NORMAL_SAMPLE_NAME \
  --input $TUMOR_BAM_FILE \
  --tumor-sample $TUMOR_SAMPLE_NAME \
  --output $VCF_OUTPUT_FILE

  As variant calling was performed on given samples same samples were used in the script which is added as "vcf.sh" .
  Output VCF file is also attached for reference.

  Variant Annotation Using VEP 

  Command used : 

  $ /ensembl-vep_updated/ensembl-vep/vep -i variant.vcf -o annotated.vcf --gtf gencode.v42.annotation.gtf.gz --fasta hg38.fa.gz --symbol Genesymbol

  Annotated file is attached as "annotated.txt"

