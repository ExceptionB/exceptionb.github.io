
<!DOCTYPE html>
<html lang="zh-cn" class="loading">
<head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
    <meta name="viewport" content="width=device-width, minimum-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Crypto-WriteUps (BuuCTF) - ExceptionB`s Small Room</title>
    <meta name="apple-mobile-web-app-capable" content="yes" />
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
    <meta name="google" content="notranslate" />
    <meta name="keywords" content="Blog,"> 
    <meta name="description" content="BUUCTF做题记录Crypto1.MD5反查md5秒杀
flag&amp;#123;admin1&amp;#125;
2.一眼就解密base64秒杀
flag&amp;#123;THE_FLAG_OF_THIS_STRI,"> 
    <meta name="author" content="ExceptionB Ch. (aka 鲤唐可可)"> 
    <link rel="alternative" href="atom.xml" title="ExceptionB`s Small Room" type="application/atom+xml"> 
    <link rel="icon" href="/img/favicon.png"> 
    
    
    
    <meta name="twitter:card" content="summary"/>
    <meta name="twitter:title" content="Crypto-WriteUps (BuuCTF) - ExceptionB`s Small Room"/>
    <meta name="twitter:description" content="BUUCTF做题记录Crypto1.MD5反查md5秒杀
flag&amp;#123;admin1&amp;#125;
2.一眼就解密base64秒杀
flag&amp;#123;THE_FLAG_OF_THIS_STRI,"/>
    
    
    
    
    <meta property="og:site_name" content="ExceptionB`s Small Room"/>
    <meta property="og:type" content="object"/>
    <meta property="og:title" content="Crypto-WriteUps (BuuCTF) - ExceptionB`s Small Room"/>
    <meta property="og:description" content="BUUCTF做题记录Crypto1.MD5反查md5秒杀
flag&amp;#123;admin1&amp;#125;
2.一眼就解密base64秒杀
flag&amp;#123;THE_FLAG_OF_THIS_STRI,"/>
    
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
    <h3 class="subtitle">Crypto-WriteUps (BuuCTF)</h3>
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
        <h1 class="title">Crypto-WriteUps (BuuCTF)</h1>
        <div class="stuff">
            <span>十月 01, 2022</span>
            

        </div>
        <div class="content markdown">
            <h1 id="BUUCTF做题记录"><a href="#BUUCTF做题记录" class="headerlink" title="BUUCTF做题记录"></a>BUUCTF做题记录</h1><h2 id="Crypto"><a href="#Crypto" class="headerlink" title="Crypto"></a>Crypto</h2><h3 id="1-MD5"><a href="#1-MD5" class="headerlink" title="1.MD5"></a>1.MD5</h3><p>反查md5秒杀</p>
<p><code>flag&#123;admin1&#125;</code></p>
<h3 id="2-一眼就解密"><a href="#2-一眼就解密" class="headerlink" title="2.一眼就解密"></a>2.一眼就解密</h3><p>base64秒杀</p>
<p><code>flag&#123;THE_FLAG_OF_THIS_STRING&#125;</code></p>
<h3 id="3-Url编码"><a href="#3-Url编码" class="headerlink" title="3.Url编码"></a>3.Url编码</h3><p>url编码秒杀</p>
<p><code>flag&#123;and 1=1&#125;</code></p>
<h3 id="4-看我回旋踢"><a href="#4-看我回旋踢" class="headerlink" title="4.看我回旋踢"></a>4.看我回旋踢</h3><p>简单的凯撒密码秒杀<br>offset=n</p>
<p><code>flag&#123;5cd1004d-86a5-46d8-b720-beb5ba0417e1&#125;</code></p>
<h3 id="5-摩丝"><a href="#5-摩丝" class="headerlink" title="5.摩丝"></a>5.摩丝</h3><p>摩斯电码秒杀</p>
<p><code>flag&#123;ILOVEYOU&#125;</code></p>
<h3 id="6-password"><a href="#6-password" class="headerlink" title="6.password"></a>6.password</h3><p>全靠猜</p>
<p><code>flag&#123;zs19900315&#125;</code></p>
<h3 id="7-变异凯撒"><a href="#7-变异凯撒" class="headerlink" title="7.变异凯撒"></a>7.变异凯撒</h3><p>我的评价是 发病<br>先转为ASCII，然后依次加5，6，7，8……</p>
<p><code>flag&#123;Caesar_variation&#125;</code></p>
<h3 id="8-Quoted-printable"><a href="#8-Quoted-printable" class="headerlink" title="8.Quoted-printable"></a>8.Quoted-printable</h3><p>Quoted-printable解码工具秒杀</p>
<p><code>flag&#123;那你也很棒哦&#125;</code></p>
<h3 id="9-Rabbit"><a href="#9-Rabbit" class="headerlink" title="9.Rabbit"></a>9.Rabbit</h3><p>rabbit对称加密秒杀<br>空密码</p>
<p><code>flag&#123;Cute_Rabbit&#125;</code></p>
<h3 id="10-篱笆墙的影子"><a href="#10-篱笆墙的影子" class="headerlink" title="10.篱笆墙的影子"></a>10.篱笆墙的影子</h3><p>栅栏密码秒杀<br>每组13字</p>
<p><code>flag&#123;wethinkwehavetheflag&#125;</code></p>
<h3 id="11-RSA"><a href="#11-RSA" class="headerlink" title="11.RSA"></a>11.RSA</h3><p>标准的RSA流程，秒杀</p>
<p><code>flag&#123;125631357777427553&#125;</code></p>
<h3 id="12-丢失的MD5"><a href="#12-丢失的MD5" class="headerlink" title="12.丢失的MD5"></a>12.丢失的MD5</h3><p>直接运行附件就可以了</p>
<p><code>flag&#123;e9032994dabac08080091151380478a2&#125;</code></p>
<h3 id="13-Alice与Bob"><a href="#13-Alice与Bob" class="headerlink" title="13.Alice与Bob"></a>13.Alice与Bob</h3><p>数很小，直接分解算md5，秒杀</p>
<p><code>flag&#123;d450209323a847c8d01c6be47c81811a&#125;</code></p>
<h3 id="14-rsarsa"><a href="#14-rsarsa" class="headerlink" title="14.rsarsa"></a>14.rsarsa</h3><p>标准的RSA，秒杀</p>
<p><code>flag&#123;5577446633554466577768879988&#125;</code></p>
<h3 id="15-大帝的密码武器"><a href="#15-大帝的密码武器" class="headerlink" title="15.大帝的密码武器"></a>15.大帝的密码武器</h3><p>读题得知是凯撒密码，试错法得到offset=n<br>加密ComeChina得到flag</p>
<p><code>flag&#123;PbzrPuvan&#125;</code></p>
<h3 id="16-Windows系统密码"><a href="#16-Windows系统密码" class="headerlink" title="16.Windows系统密码"></a>16.Windows系统密码</h3><p>还是发病，一个个查md5，查到其中有一个是flag</p>
<p><code>flag&#123;good-luck&#125;</code></p>
<h3 id="17-凯撒？替换？呵呵"><a href="#17-凯撒？替换？呵呵" class="headerlink" title="17.凯撒？替换？呵呵!"></a>17.凯撒？替换？呵呵!</h3><p>quipqiup一键爆破</p>
<p><code>flag&#123;substitutioncipherdecryptionisalwayseasyjustlikeapieceofcake&#125;</code></p>
<h3 id="18-萌萌哒的八戒"><a href="#18-萌萌哒的八戒" class="headerlink" title="18.萌萌哒的八戒"></a>18.萌萌哒的八戒</h3><p>明显的猪圈密码，秒杀</p>
<p><code>flag&#123;whenthepigwanttoeat&#125;</code></p>
<h3 id="19-权限获得第一步"><a href="#19-权限获得第一步" class="headerlink" title="19.权限获得第一步"></a>19.权限获得第一步</h3><p>反查md5秒杀</p>
<p><code>flag&#123;3617656&#125;</code></p>
<h3 id="20-RSA1"><a href="#20-RSA1" class="headerlink" title="20.RSA1"></a>20.RSA1</h3><p>用中国剩余定理求d</p>
<p><code>flag&#123;W31c0m3_70_Ch1n470wn&#125;</code></p>
<h3 id="21-old-fashion"><a href="#21-old-fashion" class="headerlink" title="21.old-fashion"></a>21.old-fashion</h3><p>一眼鉴定为维吉尼亚密码，但是需要手动判断一些线索<br>用quipqiup进行破解<br>多次尝试，得到线索为</p>
<figure class="highlight plaintext"><table><tr><td class="gutter"><pre><span class="line">1</span><br><span class="line">2</span><br><span class="line">3</span><br><span class="line">4</span><br><span class="line">5</span><br></pre></td><td class="code"><pre><span class="line">OS=BY</span><br><span class="line">mjy vrwm qrvvrf=the most common</span><br><span class="line">Wr=So</span><br><span class="line">dsln=flag</span><br><span class="line">bw=is</span><br></pre></td></tr></table></figure>
<p>最后就得到flag了</p>
<p><code>flag&#123;n1_2hen-d3_hu1-mi-ma_a&#125;</code></p>
<h3 id="22-世上无难事"><a href="#22-世上无难事" class="headerlink" title="22.世上无难事"></a>22.世上无难事</h3><p>一眼鉴定为维吉尼亚密码，用quipqiup进行破解，秒杀</p>
<p><code>flag&#123;640e11012805f211b0ab24ff02a1ed09&#125;</code></p>
<h3 id="23-RSA3"><a href="#23-RSA3" class="headerlink" title="23.RSA3"></a>23.RSA3</h3><p>泄露dp dq，一眼鉴定为RSA共模攻击，套模板秒杀</p>
<p><code>flag&#123;49d91077a1abcb14f1a9d546c80be9ef&#125;</code></p>
<h3 id="24-RSA2"><a href="#24-RSA2" class="headerlink" title="24.RSA2"></a>24.RSA2</h3><p>泄露dp，尝试分解n，然后常规解法</p>
<p><code>flag&#123;wow_leaking_dp_breaks_rsa?_98924743502&#125;</code></p>
<h3 id="25-Unencode"><a href="#25-Unencode" class="headerlink" title="25.Unencode"></a>25.Unencode</h3><p>是UUencode，直接一键解码</p>
<p><code>flag&#123;dsdasdsa99877LLLKK&#125;</code></p>
<h3 id="26-AFCTF2018-Morse"><a href="#26-AFCTF2018-Morse" class="headerlink" title="26.[AFCTF2018]Morse"></a>26.[AFCTF2018]Morse</h3><p>看题目得知是摩斯电码，一键解码得到<br><code>61666374667B317327745F73305F333435797D</code><br>作为flag提交，发现错误<br>观察字符集，考虑可能是HEX，解码后得到flag</p>
<p><code>flag&#123;1s&#39;t_s0_345y&#125;</code></p>
<h3 id="27-异性相吸"><a href="#27-异性相吸" class="headerlink" title="27.异性相吸"></a>27.异性相吸</h3><p>读题猜测是XOR，秒杀</p>
<p><code>flag&#123;ea1bc0988992276b7f95b54a7435e89e&#125;</code></p>
<h3 id="28-还原大师"><a href="#28-还原大师" class="headerlink" title="28.还原大师"></a>28.还原大师</h3><p>题目都说到这里了，那就直接爆破呗，反正也就26^3种可能</p>
<figure class="highlight python"><table><tr><td class="gutter"><pre><span class="line">1</span><br><span class="line">2</span><br><span class="line">3</span><br><span class="line">4</span><br><span class="line">5</span><br><span class="line">6</span><br><span class="line">7</span><br><span class="line">8</span><br><span class="line">9</span><br><span class="line">10</span><br><span class="line">11</span><br><span class="line">12</span><br><span class="line">13</span><br><span class="line">14</span><br><span class="line">15</span><br><span class="line">16</span><br><span class="line">17</span><br><span class="line">18</span><br><span class="line">19</span><br><span class="line">20</span><br><span class="line">21</span><br><span class="line">22</span><br><span class="line">23</span><br></pre></td><td class="code"><pre><span class="line"><span class="keyword">from</span> hashlib <span class="keyword">import</span> md5</span><br><span class="line"></span><br><span class="line"><span class="keyword">def</span> <span class="title function_">cmp</span>(<span class="params">a,b</span>):</span><br><span class="line">    <span class="keyword">if</span> <span class="keyword">not</span> <span class="built_in">len</span>(a) == <span class="built_in">len</span>(b):</span><br><span class="line">        <span class="keyword">return</span> <span class="literal">False</span></span><br><span class="line">    <span class="keyword">for</span> x <span class="keyword">in</span> <span class="built_in">range</span>(<span class="built_in">len</span>(a)):</span><br><span class="line">        <span class="keyword">if</span> a[x] == <span class="string">&quot;?&quot;</span>:</span><br><span class="line">            <span class="keyword">continue</span></span><br><span class="line">        <span class="keyword">elif</span> <span class="keyword">not</span> a[x] == b[x]:</span><br><span class="line">            <span class="keyword">return</span> <span class="literal">False</span></span><br><span class="line">    <span class="keyword">return</span> <span class="literal">True</span></span><br><span class="line"></span><br><span class="line">words = <span class="string">&quot;QWERTYUIOPASDFGHJKLZXCVBNM&quot;</span></span><br><span class="line">pattern = <span class="string">&quot;E903???4DAB????08?????51?80??8A?&quot;</span>.lower()</span><br><span class="line"></span><br><span class="line"><span class="keyword">for</span> a <span class="keyword">in</span> words:</span><br><span class="line">    <span class="keyword">for</span> b <span class="keyword">in</span> words:</span><br><span class="line">        <span class="keyword">for</span> c <span class="keyword">in</span> words:</span><br><span class="line">            i = <span class="string">&quot;TASC%sO3RJMV%sWDJKX%sZM&quot;</span>%(a,b,c)</span><br><span class="line">            m = md5(i.encode()).hexdigest()</span><br><span class="line">            <span class="keyword">if</span> cmp(pattern,m):</span><br><span class="line">                <span class="built_in">print</span>(m)</span><br><span class="line"></span><br></pre></td></tr></table></figure>

<p><code>flag&#123;E9032994DABAC08080091151380478A2&#125;</code></p>
<h3 id="29-RSA"><a href="#29-RSA" class="headerlink" title="29.RSA"></a>29.RSA</h3><p>题目给了密文和一个公钥文件，首先从公钥文件中读出n, e</p>
<figure class="highlight python"><table><tr><td class="gutter"><pre><span class="line">1</span><br><span class="line">2</span><br><span class="line">3</span><br><span class="line">4</span><br><span class="line">5</span><br></pre></td><td class="code"><pre><span class="line"><span class="keyword">from</span> Crypto.PublicKey <span class="keyword">import</span> RSA</span><br><span class="line"><span class="keyword">with</span> <span class="built_in">open</span>(<span class="string">&quot;./downloads/pub.key&quot;</span>,<span class="string">&#x27;r&#x27;</span>) <span class="keyword">as</span> fs:</span><br><span class="line">    k = RSA.import_key(fs.read())</span><br><span class="line">    <span class="built_in">print</span>(k.e)</span><br><span class="line">    <span class="built_in">print</span>(k.n)</span><br></pre></td></tr></table></figure>
<p>然后就是标准的RSA</p>
<p><code>flag&#123;decrypt_256&#125;</code></p>
<h3 id="30-RSAROLL"><a href="#30-RSAROLL" class="headerlink" title="30.RSAROLL"></a>30.RSAROLL</h3><p>我的评价是，抽象艺术</p>
<p>题目的第一行，通过猜测可知，一个是n，一个是e<br>下面的一堆数字，都是加密后的文本，那么就一个一个的解码，然后拼在一起，就是flag了</p>
<p><code>flag&#123;13212je2ue28fy71w8u87y31r78eu1e2&#125;</code></p>
<h3 id="31-Dangerous-RSA"><a href="#31-Dangerous-RSA" class="headerlink" title="31.Dangerous RSA"></a>31.Dangerous RSA</h3><p>RSA小公钥指数攻击，秒杀</p>
<p><code>flag&#123;25df8caf006ee5db94d48144c33b2c3b&#125;</code></p>
<h3 id="32-Cipher"><a href="#32-Cipher" class="headerlink" title="32.Cipher"></a>32.Cipher</h3><p>有种古典密码，叫做playfair……</p>
<p><code>flag&#123;itisnotaproblemhavefun&#125;</code></p>
<h3 id="33-HDCTF2019-basic-rsa"><a href="#33-HDCTF2019-basic-rsa" class="headerlink" title="33.[HDCTF2019]basic rsa"></a>33.[HDCTF2019]basic rsa</h3><p>给了pqec，那就是最简单的rsa</p>
<p><code>flag&#123;B4by_Rs4&#125;</code></p>
<h3 id="34-GUET-CTF2019-BabyRSA"><a href="#34-GUET-CTF2019-BabyRSA" class="headerlink" title="34.[GUET-CTF2019]BabyRSA"></a>34.[GUET-CTF2019]BabyRSA</h3><p>给了p+q和(p+1)(q+1)，求得n=p*q，然后就秒杀了</p>
<p><code>flag&#123;cc7490e-78ab-11e9-b422-8ba97e5da1fd&#125;</code></p>
<h3 id="35-密码学的心声"><a href="#35-密码学的心声" class="headerlink" title="35.密码学的心声"></a>35.密码学的心声</h3><p>歌词都提示到这里了，一看就是八进制</p>
<p><code>flag&#123;ILoveSecurityVeryMuch&#125;</code></p>
<h3 id="36-BJDCTF2020-这是base"><a href="#36-BJDCTF2020-这是base" class="headerlink" title="36.[BJDCTF2020]这是base??"></a>36.[BJDCTF2020]这是base??</h3><p>确实是base64，只不过顺序不太一样，根据题目附的词典，得到alphabet为<code>JKLMNOxyUVzABCDEFGH789PQIabcdefghijklmWXYZ0123456RSTnopqrstuvw</code></p>
<p><code>flag&#123;D0_Y0u_kNoW_Th1s_b4se_map&#125;</code></p>
<h3 id="37-rsa2"><a href="#37-rsa2" class="headerlink" title="37.rsa2"></a>37.rsa2</h3><p>yysy，这个求d很简单，在线分解N得到p q，然后常规方法就可以得到d<br>但是这里涉及到python2与python3之间的一些差别，在查阅资料后发现，python3的hex()输出比python2少了末尾的一个’L’，要手动补上才可以</p>
<p><code>flag&#123;47bf28da384590448e0b0d23909a25a4&#125;</code></p>
<h3 id="38-RSA5"><a href="#38-RSA5" class="headerlink" title="38.RSA5"></a>38.RSA5</h3><p>在一群的n里面，恰好有一对n，不互质，且最大公约数为质数，于是就把这个n分解出来了，然后常规解法</p>
<p><code>flag&#123;abdcbe5fd94e23b3de429223ab9c2fdf&#125;</code></p>
<h3 id="39-WUSTCTF2020-佛说：只能四天"><a href="#39-WUSTCTF2020-佛说：只能四天" class="headerlink" title="39.[WUSTCTF2020]佛说：只能四天"></a>39.[WUSTCTF2020]佛说：只能四天</h3><p>这是真的要脑洞的古典密码。<br>看到题目，第一反应是，与佛论禅。根据描述中的旧约和新约，知道这个是新约的与佛论禅。<br>解密后，明显是个社会主义加密，解密后，发现最后带了一串提示，可知又有栅栏加密，尝试了几个栅栏大小后，发现在栅栏大小为4时，得到下一步是凯撒加密。<br>凯撒密码默认位移是三，解密后得到一串字母与数字混合的字符串。<br>根据提示，凯撒不是最后一个，又没有更多提示，只能开始猜。根据字符集，先排除了Hex，而且字母并不是大小写都有，也可以排除base64等。<br>尝试Base32，<del>蒙对了</del></p>
<p><code>flag&#123;ni_hao_xiang_xiang_da_wo&#125;</code></p>
<h3 id="40-NCTF2019-childRSA"><a href="#40-NCTF2019-childRSA" class="headerlink" title="40.[NCTF2019]childRSA"></a>40.[NCTF2019]childRSA</h3><p>平滑数，后面的我忘了（</p>
<p><code>flag&#123;Th3r3_ar3_1ns3cure_RSA_m0duli_7hat_at_f1rst_gl4nce_appe4r_t0_be_s3cur3&#125;</code></p>
<h3 id="41-这是什么"><a href="#41-这是什么" class="headerlink" title="41.这是什么"></a>41.这是什么</h3><p>看到这个apk还下了一跳，用7zip打开后发现是.doc格式<br>这叫什么加密我忘了，反正直接丢到控制台里面执行就好了（</p>
<p><code>flag&#123;a0448fd730b62c13ca80200c4529daa2&#125;</code></p>
<h3 id="42-HDCTF2019-bbbbbbrsa"><a href="#42-HDCTF2019-bbbbbbrsa" class="headerlink" title="42.[HDCTF2019]bbbbbbrsa"></a>42.[HDCTF2019]bbbbbbrsa</h3><p>题目给了p n c，那么q也是已知的，只要找出e即可。<br>因为题目中的e是个随机生成的与phi互质的数，由于其范围不大，所以可以枚举从50000到70000的所有数，找到满足与phi互质的e进行解密，最后筛选就可以得到flag了。（满足的e有5579个，只有一个解密结果以flag开头，<del>计算量不大，11s就算完了</del>）</p>
<p><code>flag&#123;rs4_1s_s1mpl3!#&#125;</code></p>
<h3 id="43-BJDCTF2020-RSA"><a href="#43-BJDCTF2020-RSA" class="headerlink" title="43.[BJDCTF2020]RSA"></a>43.[BJDCTF2020]RSA</h3><p>读题，题目给了两组n c，并且两个n有一个共因数q，且q为素数，即可计算得到p1 p2。<br>此时还差e是未知数，但由于题目给了两个条件：</p>
<ol>
<li><code>assert(e&lt;100000)</code></li>
<li><code>print pow(294,e,n)</code></li>
</ol>
<p>那直接枚举这十万个数，找到符合条件的e即可，最后算出e=52361</p>
<p><code>flag&#123;p_is_common_divisor&#125;</code></p>

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
            <ol class="toc"><li class="toc-item toc-level-1"><a class="toc-link" href="#BUUCTF%E5%81%9A%E9%A2%98%E8%AE%B0%E5%BD%95"><span class="toc-number">1.</span> <span class="toc-text">BUUCTF做题记录</span></a><ol class="toc-child"><li class="toc-item toc-level-2"><a class="toc-link" href="#Crypto"><span class="toc-number">1.1.</span> <span class="toc-text">Crypto</span></a><ol class="toc-child"><li class="toc-item toc-level-3"><a class="toc-link" href="#1-MD5"><span class="toc-number">1.1.1.</span> <span class="toc-text">1.MD5</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#2-%E4%B8%80%E7%9C%BC%E5%B0%B1%E8%A7%A3%E5%AF%86"><span class="toc-number">1.1.2.</span> <span class="toc-text">2.一眼就解密</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#3-Url%E7%BC%96%E7%A0%81"><span class="toc-number">1.1.3.</span> <span class="toc-text">3.Url编码</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#4-%E7%9C%8B%E6%88%91%E5%9B%9E%E6%97%8B%E8%B8%A2"><span class="toc-number">1.1.4.</span> <span class="toc-text">4.看我回旋踢</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#5-%E6%91%A9%E4%B8%9D"><span class="toc-number">1.1.5.</span> <span class="toc-text">5.摩丝</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#6-password"><span class="toc-number">1.1.6.</span> <span class="toc-text">6.password</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#7-%E5%8F%98%E5%BC%82%E5%87%AF%E6%92%92"><span class="toc-number">1.1.7.</span> <span class="toc-text">7.变异凯撒</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#8-Quoted-printable"><span class="toc-number">1.1.8.</span> <span class="toc-text">8.Quoted-printable</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#9-Rabbit"><span class="toc-number">1.1.9.</span> <span class="toc-text">9.Rabbit</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#10-%E7%AF%B1%E7%AC%86%E5%A2%99%E7%9A%84%E5%BD%B1%E5%AD%90"><span class="toc-number">1.1.10.</span> <span class="toc-text">10.篱笆墙的影子</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#11-RSA"><span class="toc-number">1.1.11.</span> <span class="toc-text">11.RSA</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#12-%E4%B8%A2%E5%A4%B1%E7%9A%84MD5"><span class="toc-number">1.1.12.</span> <span class="toc-text">12.丢失的MD5</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#13-Alice%E4%B8%8EBob"><span class="toc-number">1.1.13.</span> <span class="toc-text">13.Alice与Bob</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#14-rsarsa"><span class="toc-number">1.1.14.</span> <span class="toc-text">14.rsarsa</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#15-%E5%A4%A7%E5%B8%9D%E7%9A%84%E5%AF%86%E7%A0%81%E6%AD%A6%E5%99%A8"><span class="toc-number">1.1.15.</span> <span class="toc-text">15.大帝的密码武器</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#16-Windows%E7%B3%BB%E7%BB%9F%E5%AF%86%E7%A0%81"><span class="toc-number">1.1.16.</span> <span class="toc-text">16.Windows系统密码</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#17-%E5%87%AF%E6%92%92%EF%BC%9F%E6%9B%BF%E6%8D%A2%EF%BC%9F%E5%91%B5%E5%91%B5"><span class="toc-number">1.1.17.</span> <span class="toc-text">17.凯撒？替换？呵呵!</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#18-%E8%90%8C%E8%90%8C%E5%93%92%E7%9A%84%E5%85%AB%E6%88%92"><span class="toc-number">1.1.18.</span> <span class="toc-text">18.萌萌哒的八戒</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#19-%E6%9D%83%E9%99%90%E8%8E%B7%E5%BE%97%E7%AC%AC%E4%B8%80%E6%AD%A5"><span class="toc-number">1.1.19.</span> <span class="toc-text">19.权限获得第一步</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#20-RSA1"><span class="toc-number">1.1.20.</span> <span class="toc-text">20.RSA1</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#21-old-fashion"><span class="toc-number">1.1.21.</span> <span class="toc-text">21.old-fashion</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#22-%E4%B8%96%E4%B8%8A%E6%97%A0%E9%9A%BE%E4%BA%8B"><span class="toc-number">1.1.22.</span> <span class="toc-text">22.世上无难事</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#23-RSA3"><span class="toc-number">1.1.23.</span> <span class="toc-text">23.RSA3</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#24-RSA2"><span class="toc-number">1.1.24.</span> <span class="toc-text">24.RSA2</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#25-Unencode"><span class="toc-number">1.1.25.</span> <span class="toc-text">25.Unencode</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#26-AFCTF2018-Morse"><span class="toc-number">1.1.26.</span> <span class="toc-text">26.[AFCTF2018]Morse</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#27-%E5%BC%82%E6%80%A7%E7%9B%B8%E5%90%B8"><span class="toc-number">1.1.27.</span> <span class="toc-text">27.异性相吸</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#28-%E8%BF%98%E5%8E%9F%E5%A4%A7%E5%B8%88"><span class="toc-number">1.1.28.</span> <span class="toc-text">28.还原大师</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#29-RSA"><span class="toc-number">1.1.29.</span> <span class="toc-text">29.RSA</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#30-RSAROLL"><span class="toc-number">1.1.30.</span> <span class="toc-text">30.RSAROLL</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#31-Dangerous-RSA"><span class="toc-number">1.1.31.</span> <span class="toc-text">31.Dangerous RSA</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#32-Cipher"><span class="toc-number">1.1.32.</span> <span class="toc-text">32.Cipher</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#33-HDCTF2019-basic-rsa"><span class="toc-number">1.1.33.</span> <span class="toc-text">33.[HDCTF2019]basic rsa</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#34-GUET-CTF2019-BabyRSA"><span class="toc-number">1.1.34.</span> <span class="toc-text">34.[GUET-CTF2019]BabyRSA</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#35-%E5%AF%86%E7%A0%81%E5%AD%A6%E7%9A%84%E5%BF%83%E5%A3%B0"><span class="toc-number">1.1.35.</span> <span class="toc-text">35.密码学的心声</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#36-BJDCTF2020-%E8%BF%99%E6%98%AFbase"><span class="toc-number">1.1.36.</span> <span class="toc-text">36.[BJDCTF2020]这是base??</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#37-rsa2"><span class="toc-number">1.1.37.</span> <span class="toc-text">37.rsa2</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#38-RSA5"><span class="toc-number">1.1.38.</span> <span class="toc-text">38.RSA5</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#39-WUSTCTF2020-%E4%BD%9B%E8%AF%B4%EF%BC%9A%E5%8F%AA%E8%83%BD%E5%9B%9B%E5%A4%A9"><span class="toc-number">1.1.39.</span> <span class="toc-text">39.[WUSTCTF2020]佛说：只能四天</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#40-NCTF2019-childRSA"><span class="toc-number">1.1.40.</span> <span class="toc-text">40.[NCTF2019]childRSA</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#41-%E8%BF%99%E6%98%AF%E4%BB%80%E4%B9%88"><span class="toc-number">1.1.41.</span> <span class="toc-text">41.这是什么</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#42-HDCTF2019-bbbbbbrsa"><span class="toc-number">1.1.42.</span> <span class="toc-text">42.[HDCTF2019]bbbbbbrsa</span></a></li><li class="toc-item toc-level-3"><a class="toc-link" href="#43-BJDCTF2020-RSA"><span class="toc-number">1.1.43.</span> <span class="toc-text">43.[BJDCTF2020]RSA</span></a></li></ol></li></ol></li></ol>
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
