---
hidden: true
---

<center>
  <img src="https://s3.bmp.ovh/imgs/2025/08/12/46d026b396bb06e3.png" alt="">
  <h1>此处是朋友的家</h1>
  <p><em>每一次重新造访，房屋的分布都会发生变化。</em></p>
</center>

<br/>

<!-- 友链容器：每条单独一个 .friend -->
<center>
  <div id="friends" style="max-width:700px;">
    <div class="friend">🍊 <a href="https://atlantic-wildebeest-a4c.notion.site/AWAY-251ee229cc7d8045a902e0a2ff63a5a1" target="_blank">AWAY!!</a></div>
    <div class="friend">🛢️ <a href="https://furouto.flowus.cn/" target="_blank">浮浪都</a></div>
    <div class="friend">🪗 <a href="https://ccnn1258.top/" target="_blank">鸥鹭风云</a></div>
    <div class="friend">🍐 <a href="https://harushuura.vip/" target="_blank">春天与阿修罗</a></div>
    <div class="friend">🪽 <a href="https://naturaleki.one/" target="_blank">天堂错误文件</a></div>
    <div class="friend">😰 <a href="https://ryihuan.github.io/" target="_blank">某人的小窝</a></div>
    <div class="friend">😈 <a href="https://www.asecarc.top/" target="_blank">你留下点希望的影像吧</a></div>
    <div class="friend">🦋 <a href="https://indigo-coconut-a6e.notion.site/Roaring-Roaming-9592a7fadd054c269d5109f49fb56229" target="_blank">Roaring, Roaming</a></div>
    <div class="friend">🍬 <a href="https://writee.org/wu-tang-ying-tang/" target="_blank">无糖硬糖</a></div>
    <div class="friend">🫧 <a href="https://blog.gulugulurave.com/" target="_blank">咕噜咕庐</a></div>
    <div class="friend">🌌 <a href="https://kageji.blog/" target="_blank">晷影空间站</a></div>
    <div class="friend">✈️ <a href="https://banshou-air.netlify.app/" target="_blank">夜航南飞</a></div>
    <div class="friend">🐳 <a href="https://mantyke.icu/" target="_blank">小球飞鱼</a></div>
    <div class="friend">👾 <a href="https://alanone.top/" target="_blank">ENCOM一号机</a></div>
    <div class="friend">🌊 <a href="https://imasugu.cc/" target="_blank">東井</a></div>
    <div class="friend">🔮 <a href="https://writee.org/erythrina/" target="_blank">Ery的魔法大鍋</a></div>
    <div class="friend">🪴 <a href="https://kujira-tiku.vercel.app/" target="_blank">清熱鯨騰草</a></div>
    <div class="friend">🐾 <a href="https://u-mok.blog/" target="_blank">此獠当诛第一名</a></div>
  </div>
</center>

<br/>

<center><img src="https://s3.bmp.ovh/imgs/2025/12/16/6b4a6db94ea5153a.png" alt=""></center>

<br/>

<style>
  /* 容器：居中 + 垂直排列 + 间距 */
  #friends {
    max-width: 700px;
    margin: 0 auto;              /* 容器水平居中（保留 <center> 也可以） */
    display: flex;
    flex-direction: column;      /* 垂直排列每一项 */
    align-items: center;         /* 每一项内容居中 */
    gap: 18px;                   /* 每两条之间的垂直间距（可改为 16px/20px） */
    padding: 8px 16px;
    box-sizing: border-box;
  }

  /* 每一项占满容器宽度但内部文字居中 */
  #friends .friend {
    width: 100%;
    text-align: center;          /* emoji + 链接都居中 */
    font-size: 1.05rem;
    padding: 8px 12px;           /* 项内边距，让视觉更舒展 */
    box-sizing: border-box;
  }

  #friends .friend a {
    text-decoration: none;
    display: inline-block;       /* 方便设置 padding / hover */
  }

</style>


<script>
document.addEventListener('DOMContentLoaded', function () {
  // 先解析 emoji 为 Twemoji（如果你保留 twemoji）
  if (typeof twemoji !== 'undefined') twemoji.parse(document.body);

  const container = document.getElementById('friends');
  if (!container) return;

  // 取出所有子元素并做 Fisher-Yates 随机打乱
  const items = Array.from(container.children);
  for (let i = items.length - 1; i > 0; i--) {
    const j = Math.floor(Math.random() * (i + 1));
    [items[i], items[j]] = [items[j], items[i]];
  }

  // 重新按随机顺序附加到容器（appendChild 会把原节点移动而非复制）
  items.forEach(el => container.appendChild(el));
});
</script>
