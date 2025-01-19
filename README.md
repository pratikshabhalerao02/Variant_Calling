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

  As variant calling was performed on given samples same was used in script which is added as vcf.sh 
