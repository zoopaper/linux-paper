# Linux压缩解压缩

### 1.gzip

**参数**

*   -a或–ascii 　使用ASCII文字模式。*   -c或–stdout或–to-stdout 　把压缩后的文件输出到标准输出设备，不去更动原始文件。*   -d或–decompress或—-uncompress 　解开压缩文件。*   -f或–force 　强行压缩文件。不理会文件名称或硬连接是否存在以及该文件是否为符号连接。*   -h或–help 　在线帮助。*   -l或–list 　列出压缩文件的相关信息。*   -L或–license 　显示版本与版权信息。*   -n或–no-name 　压缩文件时，不保存原来的文件名称及时间戳记。*   -N或–name 　压缩文件时，保存原来的文件名称及时间戳记。*   -q或–quiet 　不显示警告信息。*   -r或–recursive 　递归处理，将指定目录下的所有文件及子目录一并处理。*   -S&lt;压缩字尾字符串&gt;或—-suffix&lt;压缩字尾字符串&gt; 　更改压缩字尾字符串。*   -t或–test 　测试压缩文件是否正确无误。*   -v或–verbose 　显示指令执行过程。*   -V或–version 　显示版本信息。*   -&lt;压缩效率&gt; 　压缩效率是一个介于1－9的数值，预设值为”6″，指定愈大的数值，压缩效率就会愈高。*   –best 　此参数的效果和指定”-9″参数相同。*   –fast 　此参数的效果和指定”-1″参数相同。

**实例**

     <span class="hljs-number">1</span>. 压缩并删除原文件
        gzip file<span class="hljs-class">.txt</span>

     <span class="hljs-number">2</span>. 压缩不删除原文件
        gizp -c file<span class="hljs-class">.txt</span> >./file<span class="hljs-class">.gz</span>

     <span class="hljs-number">3</span>. 压缩目录中所有文件(*不能压缩整个目录*)
        gzip -r soft

     <span class="hljs-number">3</span>.快速压缩，代价是压缩比最高  
        gzip -c --fast artile<span class="hljs-class">.csv</span> >./<span class="hljs-tag">article</span><span class="hljs-class">.gz</span>

     <span class="hljs-number">4</span>.解压缩
        gzip -d <span class="hljs-tag">article</span>.gz
    