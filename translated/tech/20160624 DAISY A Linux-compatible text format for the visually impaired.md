DAISY : 一种服务视力缺陷者的linux文本格式
=================================================================


![](https://opensource.com/sites/default/files/styles/image-full-size/public/images/education/osdc-lead_books.png?itok=K8wqfPT5)
>图片: 
由Kate Ter Haar提供图片. opensource.com. CC BY-SA 2.0后期修饰

如果你像我一样是一个盲人或者有视力障碍，你经常会为了看见人们认为理所应当看得见的东西而要求不同层次的软件或硬件。 在这其中就有为阅读印刷图书的专用格式： 盲字印（假设你知道怎样阅读它）或 特殊的文本格式例如DAISY.

### DAISY是什么？
DAISY代表着一种数字化无障碍信息系统。 它是一种开方的标准，专用于服务盲人阅读教科书，杂志，报纸，小说等。 它是在90年代中期被一个叫[小雏菊联盟][1]的组织发明，这个组织致力于创造出一套进行文本标记的标准，它可以使得特殊群体像视觉正常的人一样，更加容易的阅读，跳过内容，进行注释和其他文本操作。

现在的DAISY 3.0版本是在2005年中期发布的，是一个完整的重写的标准。 它以更加容易遵守规范进行写书的目的被创造出来。 值得注意的是，DAISY仅支持纯文本，录音（PCM波形文件格式或者MPEG播放器的III格式），或文本和录音的组合。专业化的软件能阅读这类书并支持设置书签，使得视力缺陷者像正常人一样阅读印刷书籍。

### DAISY是怎样工作的呢？
DAISY, 忽略特别的版本，它工作时有点像这样： 读者拥有自己的向导文件（DAISY 2.02中的ncc.html），它包含书籍的元数据，比如作者的姓名，版权信息，书籍的页数等等。在DAISY 3.0中他是一种有效的XML文件，和DTD(文档类型定义)被强烈建议包含在每一本书中。

在导航控制文件中，标记精确描述了各个位置——无论是文本导航中插入符号的偏移量还是录音中定位至毫秒，这让软件像视力健康的人一样准确定位到相关的位置。值得注意的是这种导航文件仅有书中主要的，重要的内容的位置。

最小的内容部分由SMIL（同步多媒体集成语言）处理。导航的质量很大程度上决定于书籍的标记。这样设想一下，如果书籍没有章节标题，你需要花很多的时间来确定自己阅读的位置。如果一本DAISY格式的书籍被标记的很差， 你可能只能到书本的开头或者目录。如果书籍被标记的很差（或者完全丢失了标记），你的DAISY阅读软件很可能会简单的忽略它。

### 为什么需要专门的软件?
如果DAISY仅仅是HTML，XML,录音文件，还需要使用专门的软件进行阅读和操作，你可能会问为什么。单纯从技术上而言，你并不需要。专业化的软件大多数情况下是为了方便。这就像，在linux操作系统中，一个简单的web浏览器可以被用来打开并阅读书籍。如果你在一本DAISY 3 的书中点击XML文件，软件通常会阅读你赋予相应权限的书脊并一个你点击打开的书籍清单。如果书籍被标记的很差，它不会显示在这份清单中。

创建DAISY则完全是另一件事了，通常需要专门的软件或需要拥有足够的知识来修改软件来达到这样的目的。

### 结语
幸运的是，DAISY是一个确定了的标准。虽然它在阅读方面表现的很棒，但它需要专业软件进行生产的事实使得视力缺陷者不属于正常者看见的世界，相反这类人生活在使用各种文本格式进行电子阅读的世界中。这就是小雏菊联盟在EPUB格式上研制DAISY成功的原因，第3版，支持“媒体覆盖”。即在EPUB电子书中增加声频或视频。由于EPUB分享很多的DAISY XML标记文本，很多软件都能阅读DAISY，能看EPUB电子书但不能阅读。这也就意味着只要网站提供这种开放格式的书籍，我们将会由更多的软件选择来阅读我们的书籍。

--------------------------------------------------------------------------------

资源来自: https://opensource.com/life/16/5/daisy-linux-compatible-text-format-visually-impaired

作者：[Kendell Clark][a]
译者：[theArcticOcean](https://github.com/theArcticOcean)
校对：[校对者ID](https://github.com/校对者ID)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创翻译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://opensource.com/users/kendell-clark
[1]: http://www.daisy.org