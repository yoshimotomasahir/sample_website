---
layout: single
title: "デザイン確認"
---

## ようこそ
とある会議は、いろいろがんばってよりよくする活動をしています。

## 最近の投稿

[幹事会 議事録を掲載しました]({% post_url 2026-07-03-first-post %})
Minimal Mistakes のスキンをURLパラメータで切り替えて確認できます。

<form method="get" action="{{ "/" | relative_url }}">
  <label for="skin-select">Skin</label>
  <select id="skin-select" name="skin">
    <option value="default">default</option>
    <option value="air">air</option>
    <option value="aqua">aqua</option>
    <option value="contrast">contrast</option>
    <option value="dark">dark</option>
    <option value="dirt">dirt</option>
    <option value="mint">mint</option>
    <option value="neon">neon</option>
    <option value="plum">plum</option>
    <option value="sunrise">sunrise</option>
  </select>
  <button type="submit">Apply</button>
</form>

<script>
  (function () {
    var select = document.getElementById("skin-select");
    var skin = document.documentElement.dataset.skin || "default";
    select.value = skin;
    select.addEventListener("change", function () {
      select.form.submit();
    });
  })();
</script>

| Skin | URL |
| --- | --- |
| default | [default]({{ "/" | relative_url }}?skin=default) |
| air | [air]({{ "/" | relative_url }}?skin=air) |
| aqua | [aqua]({{ "/" | relative_url }}?skin=aqua) |
| contrast | [contrast]({{ "/" | relative_url }}?skin=contrast) |
| dark | [dark]({{ "/" | relative_url }}?skin=dark) |
| dirt | [dirt]({{ "/" | relative_url }}?skin=dirt) |
| mint | [mint]({{ "/" | relative_url }}?skin=mint) |
| neon | [neon]({{ "/" | relative_url }}?skin=neon) |
| plum | [plum]({{ "/" | relative_url }}?skin=plum) |
| sunrise | [sunrise]({{ "/" | relative_url }}?skin=sunrise) |

## 表示確認用

これは本文の表示確認用テキストです。リンク、見出し、表、引用、コードなどの見え方を確認します。

> 引用ブロックの表示確認です。

```text
sample code block
```
