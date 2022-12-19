# ldpred2_ref
Reference data for ldpred2 tool

This data originates from here:
https://figshare.com/articles/dataset/LD_reference_for_HapMap3_/21305061
(from https://privefl.github.io/bigsnpr/articles/LDpred2.html )

File ldref_hm3_plus.zip was re-downloaded, solving previous CRC issue.
MD5 sums are as follows, I believe these are correct files.

```
ce72bbe62b582ac02dd42bec019e7396  LD_with_blocks_chr10.rds
5520c1b5c07d2eb2d38c312974363990  LD_with_blocks_chr11.rds
74fa1ad91baee5eef4323043b0f92992  LD_with_blocks_chr12.rds
026e93a6302247542abffd51ef512855  LD_with_blocks_chr13.rds
efd5505c244c3c577dea7bcab1d6f10f  LD_with_blocks_chr14.rds
c7a86f79f6417030ce420d7c2c97ae28  LD_with_blocks_chr15.rds
6490d7e6df7c01efd63d9fcbfa3697f4  LD_with_blocks_chr16.rds
f2b41f30232eb6bd8607d06a6cd1189d  LD_with_blocks_chr17.rds
eaeb2fce3df89f928751f55f138b0d40  LD_with_blocks_chr18.rds
e8eb2121b7ab6371054bb9525dafe800  LD_with_blocks_chr19.rds
478a2ac9a8b94866463b9a74431489ab  LD_with_blocks_chr1.rds
8ea2f72cb733d0e52c42bc67b9e026b1  LD_with_blocks_chr20.rds
6aa555820a920c7b45b44f507ac85bd4  LD_with_blocks_chr21.rds
b1a7acdc1f13c4cb5d35cca293f0e560  LD_with_blocks_chr22.rds
2733574481c09a176de04836b642de99  LD_with_blocks_chr2.rds
e33100240e9410bf573e9675d543bb6f  LD_with_blocks_chr3.rds
fe65a230148c0be87750ad0e00da80c9  LD_with_blocks_chr4.rds
e47b6bc391cdd17d778fe59321dba3f7  LD_with_blocks_chr5.rds
a7b35d0d68ca9dfb0691fdf06ab7affc  LD_with_blocks_chr6.rds
cf51f0286f726025471125a9445c1541  LD_with_blocks_chr7.rds
78960f106da8786e1082403a2895acec  LD_with_blocks_chr8.rds
4f1b21d0c70355605ade1b94c38d1dab  LD_with_blocks_chr9.rds
```

``map_hm3_plus.justrs`` produced as follows (using R script):

```
map_ldref <- readRDS('map_hm3_plus.rds');
write.table(map_ldref$rsid, 'map_hm3_plus.justrs', row.names=F, quote=F)
```

