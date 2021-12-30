## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/Zmm-assignment/project3.github.io/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

t0.fq、t3.fq：两个不同时间段的barcodes测序数据；（下载链接：https://pan.baidu.com/s/1P-N6Gn4RbLJcrVa7zQASJQ 提取码：rlm5）
codon_table.csv：各密码子编码的氨基酸single、triple名；
barcode_reference.csv：每个barcode对应位置的密码子突变情况。
environment.yml：运行此代码所需要的环境。包含pandas 1.3.2、numpy、scipy 1.7.1、hvplot 0.7.3、panel 0.12.5、seaborn、matplotlib 3.4.3、BIO 1.3.3等packages。
Deep mutational scanning analysis：深度突变扫描是一种高通量方法，用于测量突变对蛋白质功能的影响，利用下一代测序技术在单个实验中评估蛋白质中每个位置每种可能氨基酸变化的功能后果。
DNA barcodes：在生成变体库时，将唯一的DNA条形码（barcode）与每个变体相关联，扫描所有barcodes后进行排序，以确定每个变体的富集分数。
目的：通过在酵母中对激酶Src进行深度突变扫描，检测出对Src蛋白活性具有显著影响的突变位点。Src活性越高，酵母生长越慢，而Src活性越低，酵母生长越快。
实验流程：（1）合成突变变体库（一些库将DNA条形码与每个变体相关联）。（2）将文库导入细胞（在许多情况下是酵母、细菌或噬菌体）。（3）根据蛋白质的功能进行选择，使表现良好的变体丰度增加，表现较差的变体丰度减少。（4）在选择步骤前后对编码变体的DNA或与细胞中变体相关的DNA条形码进行排序。比较每种变体的频率以计算富集率，这提供了对每种变体功能的测量。每个变量的比率是通过将所选总体中变量的频率除以其在起始或输入总体中的频率来计算的。富集比为1，表示在选择过程中变体的丰度没有变化，表明突变是中性的；富集率>1表示丰度增加，表明突变是有益的；富集率<1表示丰度减少，表明突变是有害的。
数据处理过程：（1）计算各barcode的count；（2）计算每个barcode频率；（3）计算各barcode的富集分数（以log2FC表示）；（4）计算相对于Wild type的富集分数；（5）计算氨基酸水平的富集分数；（6）绘图。
结论

# Header 1
## Header 2
### Header 3
