# From-BLAST-result-to-sequences-group

简单写了一个R脚本用来处理blast的结果，使得一群序列在blast后能够通过互相发生的hits聚成一组。
在处理转座子分类时候可能会用到，其实相应的软件能实现转座子分类的功能有很多，比如blastClust，cd-hit...
但在实际操作的时候二者的结果和直接all-to-all blast的结果是有冲突的，而且并非完全的能够实现理论上的通过相似性筛选的结果
因此我写了这个脚本
这个脚本输出的结果分别有
  *_connect_degree.xlsx(存放着序列和其同组成员产生的blast hits的数量)
  *_name.xlsx（存放着序列间的分组结果）

后续我还希望写一个基于转座子系统发育树来进行转座子分类的工具

#Translated by ChatGPT

I wrote a simple R script to process BLAST results, allowing a group of sequences to be clustered together based on mutual hits after BLAST. This may be useful when working with transposon classification. Although there are many corresponding software tools available for transposon classification, such as blastClust and cd-hit, in practice, the results of these tools often conflict with the results from a direct all-to-all BLAST, and they don't always fully achieve the theoretically expected results based on similarity filtering.
Therefore, I wrote this script.

The output of this script includes:
*_connect_degree.xlsx (containing the number of BLAST hits between each sequence and its group members)
*_name.xlsx (containing the grouping results between sequences)

In the future, I also hope to develop a tool for transposon classification based on transposon phylogenetic trees.
