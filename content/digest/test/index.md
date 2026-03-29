+++
date = '2026-03-28T17:49:51+08:00'
draft = false
title = '站点功能测试'
slug = "feature-test"
tags = ["meta"]
summary = "用于测试站点渲染效果"
+++

这是一篇用于测试 Hugo + Congo 渲染效果的文章，包含常见 Markdown 元素与程序代码。

---

## 标题

# 一级标题

## 二级标题

### 三级标题

#### 四级标题

---

## 段落与强调

这是一个普通段落。

这是 **粗体**、*斜体*、***粗斜体***。

也可以使用 `行内代码`。

~~删除线~~ 也应该正常显示。

---

## 列表

### 无序列表

- 第一项
- 第二项
  - 子项 A
  - 子项 B
- 第三项

### 有序列表

1. 第一项
2. 第二项
3. 第三项

### 任务列表

- [x] 安装 Hugo
- [x] 配置 Congo
- [ ] 写更多内容
- [ ] 加搜索功能

---

## 引用

> 这是一个引用块。
>
> Markdown 非常适合用来写个人知识库。

---

## 链接与图片

一个普通链接：

[我的主页](https://soulhacker.me/)

图片：

![成步堂龙一](gyakuten.jpg)

---

## 表格

| 名称               | 类型         | 说明     |
| ---------------- | ---------- | ------ |
| Hugo             | 静态站点生成器    | 用于生成网站 |
| Congo            | Hugo Theme | 用于页面样式 |
| Cloudflare Pages | 托管平台       | 自动部署网站 |

---

## 分隔线

上面和下面都有一条：

---

---

## 行内代码

执行下面命令启动本地预览：

```bash
hugo server -D
```

---

## 多行代码块

### Shell

```bash
git add .
git commit -m "Add markdown test article"
git push
```

### TOML

```toml
baseURL = "https://notes.example.com/"
languageCode = "zh-CN"
title = "Neo Notes"
```

### YAML

```yaml
params:
  author:
    name: "Neo Lee"
    headline: "个人 Markdown 知识库"
```

### JSON

```json
{
  "title": "Markdown Test",
  "draft": false,
  "tags": ["markdown", "test"]
}
```

### Python

```python
def greet(name: str) -> str:
    return f"Hello, {name}"

print(greet("Neo"))
```

### JavaScript

```javascript
function greet(name) {
  return `Hello, ${name}`;
}

console.log(greet("Neo"));
```

### Rust

```rust
fn main() {
    println!("Hello, Neo!");
}
```

### SQL

```sql
SELECT id, title, created_at
FROM posts
WHERE published = true
ORDER BY created_at DESC;
```

---

## 代码高亮

```diff
- old line
+ new line
```

```ini
[server]
host = localhost
port = 1313
```

```text
纯文本代码块，不带语法高亮。
```

---

## 嵌套引用与列表

> 这是一个引用。
>
> * 引用中的列表项
> * 另一项
>
> ```bash
> echo "Inside quote"
> ```

---

## Footnote

这里有一个脚注。[^1]

[^1]: 这是脚注内容。

---

## Shortcodes

来自 [Hugo](https://gohugo.io/content-management/shortcodes/) 和 [Congo](https://jpanther.github.io/congo/docs/shortcodes/) 主题支持的一些特殊标签。

### 特殊提示

Warning 图标：

{{< alert >}}
**Warning!** This action is destructive!
{{< /alert >}}

Twitter 图标：

{{< alert "x-twitter" >}}
Don't forget to [follow me](https://x.com/soulhacker) on X.
{{< /alert >}}

### Badge

{{< badge >}}新文章{{< /badge >}} 
为什么我要创建新的站点？

### 数学公式

行内公式：{{< katex >}}\(E = mc^2\)

块级公式：

{{< katex >}}
\(f(a,b,c) = (a^2+b^2+c^2)^3\)

### Mermaid

{{< mermaid >}}
graph TD
    A[Markdown] --> B[Hugo]
    B --> C[Congo]
    C --> D[Cloudflare Pages]
{{< /mermaid >}}

### Twitter

{{< x user="soulhacker" id="2034889396978401773" >}}

---

## 最后

如果这篇文章大部分都能正常显示，那么你的 Hugo + Congo + Markdown 环境应该已经基本配置好了。

