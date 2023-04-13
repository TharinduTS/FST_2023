# FST_2023

all the vcf files for different chrs are in "new_project_Apr_2023/FST/trop/VCFs"

created two text files listing males and females.

Calculating FST with

```bash
for i in Chr1 Chr2 Chr3 Chr4 Chr5 Chr6 Chr7 Chr8 Chr9 Chr10 Scafs; do vcftools --gzvcf allsites_$i*.vcf.gz --weir-fst-pop females --weir-fst-pop males --fst-window-size 5000 --fst-window-step 5000 --out ./../FST_outs/FST_F_vs_M_$i; done 
```
