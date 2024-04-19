<p>
  <img src="build/thumbnail.png" width="500" />
  <h2>Blank</h2>
  <blockquote>Absolute flexibility. All you need to let your imagination flow.</blockquote>
</p>

### ⚠️ How to use:
When you first build your page with the theme, you'll notice nothing shows up. This is intentional, as it's up to you to use the data to build your layout.

The [PRSS Client Library](https://github.com/prss-io/prss-client/blob/master/src/index.js), is already loaded with the Theme. Use its methods to render your content.

For example:
```html
<main>
    <h1></h1>
    <div class="content"></div>
</main>
<script>
    const setContent = (selector, html) => document.querySelector(selector).innerHTML = html;
    const { item } = PRSS.getAllProps();
    /*
    Returns: {
      "uuid":"fffb7461-1380-46d2-bca5-70696b1cda1c",
      "slug":"home",
      "title":"Home",
      "content":"<p>This is the beginning of something great.</p>",
      "template":"home",
      "updatedAt":1713499483159,
      "createdAt":1713390209013,
      "vars":{}
    }
    */
    setContent("h1", item.title);
    setContent(".content", item.content);
</script>

```
![image](https://github.com/prss-io/blank-theme/assets/25509135/01182596-7e65-47dd-93be-7c10599b6c3a)
![image](https://github.com/prss-io/blank-theme/assets/25509135/41397b34-1b39-4cc4-a118-c67316b7d665)
![image](https://github.com/prss-io/blank-theme/assets/25509135/0b045d89-0b9d-40f8-8d30-f2dd221a388e)

<div align="right">
  <p><a href="https://prss.io"><img src="https://i.imgur.com/5OQD7eL.png" width="130" /></a></p>
</div>
