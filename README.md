# From-BLAST-result-to-sequences-group

简单写了一个R脚本用来处理blast的结果，使得一群序列在blast后能够通过互相发生的hits聚成一组。
在处理转座子分类时候可能会用到，其实相应的软件能实现转座子分类的功能有很多，比如blastClust，cd-hit...
但在实际操作的时候二者的结果和直接all-to-all blast的结果是有冲突的，而且并非完全的能够实现理论上的通过相似性筛选的结果
因此我写了这个脚本
这个脚本输出的结果分别有
  *_connect_degree.xlsx(存放着序列和其同组成员产生的blast hits的数量)
  *_name.xlsx（存放着序列间的分组结果）
  
