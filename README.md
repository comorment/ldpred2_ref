# ldpred2_ref
Reference data for ldpred2 tool

This data originates from here:
https://figshare.com/articles/dataset/LD_reference_for_HapMap3_/21305061
(from https://privefl.github.io/bigsnpr/articles/LDpred2.html )

File ldref_hm3_plus.zip (md5sum:64b1b8658753d0af961032964a0cc747)

A strange thing is that two .rds files had bad CRC. It might be that we need to re-generated this.

```
 unzip ldref_hm3_plus.zip 
Archive:  ldref_hm3_plus.zip
 extracting: LD_with_blocks_chr1.rds  
 extracting: LD_with_blocks_chr2.rds  
 extracting: LD_with_blocks_chr3.rds  
 extracting: LD_with_blocks_chr4.rds  
 extracting: LD_with_blocks_chr5.rds   bad CRC cad8b355  (should be d7d25c5d)
 extracting: LD_with_blocks_chr6.rds  
 extracting: LD_with_blocks_chr7.rds  
 extracting: LD_with_blocks_chr8.rds  
 extracting: LD_with_blocks_chr9.rds   bad CRC b4e4afa8  (should be 75a8723b)
 extracting: LD_with_blocks_chr10.rds  
 extracting: LD_with_blocks_chr11.rds  
 extracting: LD_with_blocks_chr12.rds  
 extracting: LD_with_blocks_chr13.rds  
 extracting: LD_with_blocks_chr14.rds  
 extracting: LD_with_blocks_chr15.rds  
 extracting: LD_with_blocks_chr16.rds  
 extracting: LD_with_blocks_chr17.rds  
 extracting: LD_with_blocks_chr18.rds  
 extracting: LD_with_blocks_chr19.rds  
 extracting: LD_with_blocks_chr20.rds  
 extracting: LD_with_blocks_chr21.rds  
 extracting: LD_with_blocks_chr22.rds 
```

``map_hm3_plus.justrs`` produces as follows (using R script):

```
map_ldref <- readRDS('map_hm3_plus.rds');
write.csv(map_ldref$rsid, 'map_hm3_plus.justrs', row.names=F, quote=F)
```

