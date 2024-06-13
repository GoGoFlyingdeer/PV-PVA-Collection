# SurVis - Visual Literature Browser

![Screenshot](/doc/survis.png)

SurVis is a flexible online browser to present and analyze scientific literature. The system is made for authors of survey articles, theses, or books who want to share their references in a user-friendly way. All you need to start is a bib file and a list of keywords for your papers.

SurVis 是一个灵活的在线浏览器，用于展示和分析科学文献。该系统适用于调查文章、论文或书籍的作者，他们希望以用户友好的方式分享他们的参考文献。您只需要准备一个 bib 文件和一份关于您论文的关键词列表即可开始。

Test SurVis with a reference literature database: http://dynamicgraphs.fbeck.com

使用参考文献数据库测试 SurVis：http://dynamicgraphs.fbeck.com

## How To Use SurVis for Your Literature Collection

Dowload the latest SurVis release or fork this repository.
下载最新的 SurVis 版本或者 fork 这个存储库。

To start SurVis, open 'src/index.html' in your browser.
要启动 SurVis，请在浏览器中打开'src/index.html'。

The bibliography data is stored in 'bib/references.bib' in BibTeX format.
参考文献数据以 BibTeX 格式存储在'bib/references.bib'中。

Supplemental data is contained in 'src/data/':
补充数据包含在'src/data/'中：

- 'tag_categories.js': list of special tag categories; they can be used as a prefix for the tags and appear, for instance, 'a:b' refers to tag 'b' in tag category 'a'
- 'authorized_tags.js': tags that are defined through a description (highlighted in SurVis, description appears as a tooltip)
- 'search_stopwords.js': a list of stopwords used to exclude terms from search queries
- 'papers_pdf' (optional): PDF files of the papers, please use the BibTeX id as a file name
- 'papers_img' (optional): PNG thumbnails for the papers, please use the BibTeX id as a file name

- 'tag_categories.js'：特殊标签类别列表；它们可以用作标签的前缀，并且例如，'a:b' 指的是标签类别 'a' 中的标签 'b' 
- 'authorized_tags.js': 通过描述定义的标签（在 SurVis 中突出显示，描述显示为工具提示） 
- 'search_stopwords.js'：用于从搜索查询中排除术语的停用词列表 
- 'papers_pdf'（可选）：论文的 PDF 文件，请使用 BibTeX id 作为文件名 
- 'papers_img'（可选）：论文的 PNG 缩略图，请使用 BibTeX id 作为文件名

Please do not edit the files in 'src/data/generated/' because they are created automatically.
请不要编辑'src/data/generated/'目录中的文件，因为它们是自动生成的。

After completing your changes, just run 'update_data.py' with Python 3. Reload SurVis in the browser to see the changed bibliography. The script will continue to check for updates on the bib file until you stop it.
完成更改后，只需使用 Python 3 运行'update_data.py'。在浏览器中重新加载 SurVis 以查看更改后的参考文献。脚本将继续检查 bib 文件的更新，直到您停止它。

If the edit mode is activated, BibTeX entries can be modified in the browser, but are not stored in the 'bib' directory. To make those changes persistent, use 'download BibTex' in SurVis and copy the BibTeX data to your bib file in the 'bib' directory. You can also use the features to save and load the data from local storage of the browser; be careful, however, these features are still experimental.
如果编辑模式被激活，可以在浏览器中修改 BibTeX 条目，但不会存储在“bib”目录中。要使这些更改持久化，请在 SurVis 中使用“下载 BibTex”并将 BibTeX 数据复制到“bib”目录中的 bib 文件中。您还可以使用功能将数据保存和加载到浏览器的本地存储中；但请注意，这些功能仍处于实验阶段。

Further properties of SurVis, such as the title of the page, can be modified in the file 'src/properties.js'. For the publication of your literature collection, you should usually deactivate the edit mode in the properties ('editable = false;').
SurVis 的其他属性，如页面标题，可以在文件'src/properties.js'中进行修改。对于文献集的发布，通常应在属性中禁用编辑模式（'editable = false;'）。

Enjoy SurVis and send feedback if you like.

## Learn more

We've published a paper about SurVis at VAST 2015 - please reference it if you use or want to refer to SurVis in one of your publications.

Beck, Fabian; Koch, Sebastian; Weiskopf, Daniel: Visual Analysis and Dissemination of Scientific Literature Collections with SurVis. In: IEEE Transactions on Visualization and Computer Graphics (2015).

- DOI: http://dx.doi.org/10.1109/TVCG.2015.2467757
- Preview video: https://vimeo.com/136206061

## List of Literature Collections Using Survis

- Dynamic Graph Visualization - http://dynamicgraphs.fbeck.com
- Visualizing Group Structures in Graphs - http://go.visus.uni-stuttgart.de/groups-in-graphs/
- Performance Visualization - http://idav.ucdavis.edu/~ki/STAR/
- Visualization for Software Reuse - http://www.cos.ufrj.br/~schots/survis_reuse/
- Set Visualization - http://www.cvast.tuwien.ac.at/~alsallakh/SetViz/literature/www/index.html
- Visualizing High-Dimensional Data - http://www.sci.utah.edu/~shusenl/highDimSurvey/website/

Please contact me (fabian.beck@visus.uni-stuttgart.de) if you know other collections using SurVis.

## Contact

Fabian Beck

VISUS, University of Stuttgart

fabian.beck@visus.uni-stuttgart.de

http://research.fbeck.com
