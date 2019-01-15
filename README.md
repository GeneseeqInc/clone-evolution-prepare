# clone-evolution-prepare
此脚本用于克隆进化的文件准备，后期可使用pyclone进行克隆进化计算。

### 运行示例
```
perl clone_evolution_prepare.pl -outdir /GPFS02/home/Test -info info.csv -bamdir /GPFS02/home/Test/bam -segdir /GPFS02/home/Test/seg -fa /GPFS01/databases/GSCAP/hg19.fa -mafdir /GPFS02/home/Test/maf 
```
### 使用说明
```
==============================================================================
Description    
Options
        -outdir <s>: pathway of outdir
        -info <s>: info file
        -bamdir <s>: pathway of bam files
        -segdir <s>: pathway of seg files
        -fa : pathway of reference file
        -mafdir : pathway of maf files
	-ex : list of infos to exclude
        -h|?|help : Show this help
==============================================================================
```
### 参数解释
```
-outdir：结果输出路径
-info：病人姓名及样品对应信息，两列，第一列为病人姓名，第二列为样品名，“，”隔开
-bamdir：项目中使用的所有bam文件存放路径，须有对应的bai文件
-segdir：项目中使用的所有seg文件存放路径,seg文件可有facets输出
-mafdir：项目中使用的所有maf文件存放路径，maf文件可有vcf2maf生成
-ex：需要过滤掉的基因列表
```
