---
title: "Tasks"
date: 2023-01-04T21:55:58Z
draft: true
author: "Stephan Michard"
categories: []
tags: []

toc:
  enable: true
---

# Testing TOC 1

<!-- ft-adjustment: Adding some dummy content under each heading
for the test to work.

Just putting the headings without any content will ensure that the
test never succeeds.
Since all the headings are located in the same screen,
in a small area -->

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## Testing TOC 2

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## Testing TOC 3

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

#### Testing TOC 4

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

#### Testing TOC 5

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## Testing TOC 6

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

# Testing TOC 7

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## Testing TOC 8

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## Testing TOC 9

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

# Testing TOC 10

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

# Table of Contents

A table of content should be added to the theme. Please use the FixIt Theme for guidance ([GitHub Link](https://github.com/hugo-fixit/FixIt) and [Theme Documentation Link](https://fixit.lruihao.cn/)). The Table of contents should be displayed to the side of the post and slide up and down with the scrolling of the text.
![toc 1](/images/posts/toc_1.png)

For small windows the Table of contents should be at the top of the post in a collapsible box.
![toc 2](/images/posts/toc_2.png)

The table of contents should only be displayed for posts where the toc is enable in the frontmatter of the post:

```
toc:
  enable: true
```

# collapsible code blocks with Syntax highlighting

The code block should be collapsible, it should have a copy to clipboard button and have syntax highlighting. It should work with various types of code.
I like this implementation:
![Code Block](/images/posts/code_block.png)

## Testing code blocks

Tests:

If we consider 'collapsiblility' and 'line number' as two features of code blocks, we have the following test cases:

1. Collapsed code block with line numbers
2. Collapsed code block without line numbers
3. Expanded code block with line numbers
4. Expanded code block without line numbers
5. Code block where `lineNos` parameter is omitted
6. Code block where `isCollapsed` parameter is omitted

### 1. Collapsed code block with line numbers

Code:

```go
{{</* collapsible-code language="CSS" title="Really cool CSS snippet" isCollapsed="true" lineNos="true" */>}}
pre {
     background: #1a1a1d;
     padding: 20px;
     border-radius: 8px;
     font-size: 1rem;
     overflow: auto;
}
{{</* /collapsible-code */>}}
```

Result :

{{< collapsible-code language="CSS" title="Really cool CSS snippet" isCollapsed="true" lineNos="true">}}
pre {
     background: #1a1a1d;
     padding: 20px;
     border-radius: 8px;
     font-size: 1rem;
     overflow: auto;
}
{{< /collapsible-code >}}

### 2. Collapsed code block without line numbers

If you don't want to show line numbers, either set the `lineNos` parameter to `false` or simply omit the parameter, in which case it defaults to `false`.

Code:

```go
{{</* collapsible-code language="python" title="Really cool Python snippet" isCollapsed="true" */>}}
first_name = "Stephan"
last_name = "Michard"

print("Hello",first_name last_name,"good to see you")

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict["brand"])
{{</* /collapsible-code */>}}
```

Result:

{{< collapsible-code language="python" title="Really cool Python snippet" isCollapsed="true" >}}
first_name = "Stephan"
last_name = "Michard"

print("Hello",first_name last_name,"good to see you")

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict["brand"])
{{< /collapsible-code >}}


### 3. Expanded code block with line numbers

If you want the code to be expanded (displayed), either you can set `isCollapsed` to `false` or simply omit the parameter in which case, it defaults to  `false`

Code:

```go
{{</* collapsible-code language="CSS" title="Really cool snippet" isCollapsed="false" lineNos="true" */>}}
pre {
     background: #1a1a1d;
     padding: 20px;
     border-radius: 8px;
     font-size: 1rem;
     overflow: auto;
    }
{{</* /collapsible-code */>}}
```

Result :

{{< collapsible-code language="CSS" title="Really cool snippet" isCollapsed="false" lineNos="true" >}}
pre {
     background: #1a1a1d;
     padding: 20px;
     border-radius: 8px;
     font-size: 1rem;
     overflow: auto;
    }
{{< /collapsible-code >}}

### 4. Expanded code block without line numbers


If you want the code to be expanded and to be shown without line numbers, you can simply omit the respective parameters.

Code:

```go
{{</* collapsible-code language="python" title="Really cool Python snippet" */>}}
first_name = "Stephan"
last_name = "Michard"

print("Hello",first_name last_name,"good to see you")

print("Dear {} {}, hope you're well!".format(last_name,first_name))

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict["brand"])
{{</* /collapsible-code */>}}
```

Result:

{{< collapsible-code language="python" title="Really cool Python snippet" >}}
first_name = "Stephan"
last_name = "Michard"

print("Hello",first_name last_name,"good to see you")

print("Dear {} {}, hope you're well!".format(last_name,first_name))

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict["brand"])
{{< /collapsible-code >}}


### 5. Code block where `lineNos` parameter is omitted

When `lineNos` parameter is omitted, the default behaviour is: no line numbers shown.

Code:

```go
{{</* collapsible-code language="python" title="Really cool Python snippet" isCollapsed="true" */>}}
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict["brand"])
{{</* /collapsible-code */>}}
```

Result:

{{< collapsible-code language="python" title="Really cool Python snippet" isCollapsed="true" >}}
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict["brand"])
{{< /collapsible-code >}}

### 6. Code block where `isCollapsed` parameter is omitted

When `isCollapsed` parameter is omitted, the default behaviour is: expanded codeblock.

Code:

```go
{{</* collapsible-code language="python" title="Really cool Python snippet" lineNos="true" */>}}
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict["brand"])
{{</* /collapsible-code */>}}
```

Result:

{{< collapsible-code language="python" title="Really cool Python snippet" lineNos="true" >}}
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict["brand"])
{{< /collapsible-code >}}

## Standard code blocks

If we consider stabdard code blocks, we have 2 test cases:

1. Standard code block with line numbers
2. Standard code block without line numbers

### 1. Standard code block with line numbers

Code:

````text
```bash {linenos=true}
#!/bin/sh
mkdir dir  
mkdir -p dir_root/{dir_b}/{dir_l1,dir_l2} 
```
````

Result:

```bash {linenos=true}
#!/bin/sh
docker build --no-cache --force-rm -t site .
docker run -p 8080:8080 site

echo Some text to print out 
cat file
a=10
b=$a
let a+=10
ls
mkdir dir  
mkdir -p dir_root/{dir_b}/{dir_l1,dir_l2} 
cd dir_root
cd "dir name"
cd ~
cp file $output
```

### 2. Standard code block without line numbers

Code:

````text
```html
<div class="my_toc">
    <hr />
    <h1>Table of contents</h1>
    {{ .Page.TableOfContents }}
    <hr />
</div>
```
````

Result:

```html
<div class="my_toc">
    <hr />
    <h1>Table of contents</h1>
    {{ .Page.TableOfContents }}
    <hr />
</div>
```

## Other examples

### CSS

```css
figcaption {
 color: white;
 font-size: 1.1em;
 font-weight: 400;
 line-height: 2em;
}
```

### Javascript

```javascript
(function () {
    function onEvent() {
      var filter = search.value.toUpperCase();
      var list = document.getElementById("list");
      var filterTags = document.getElementById("list").getElementsByTagName("article");
      var listItems = list.getElementsByTagName("article");
      for (i = 0; i < listItems.length; i++) {
        var item = listItems[i];
        var textnode = listItems[i].childNodes[3].childNodes[1]
        var text = textnode.innerText.toUpperCase();
      }
    }
  })();
```

### YAML

```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: nginx-deployment
spec:
  selector:
    matchLabels:
      app: nginx
  replicas: 2 # tells deployment to run 2 pods matching the template
  template:
    metadata:
      labels:
        app: nginx
    spec:
      containers:
      - name: nginx
        image: nginx:1.14.2
        ports:
        - containerPort: 80
```

# Download File

An attachements link should be added. Instead of opening the file in the browser it should be downloaded directly. This should work for jpg and pdf files:
[Download 1](/images/posts/test_image.jpg)
[Download 2](/images/posts/test_doc.pdf)

{{< download file="/images/posts/test_doc.pdf" title="Download pdf" >}}
{{< download file="/images/posts/test_image.jpg" >}}

# Bonus: Implement nicely looking Blockquote and

I saw in your proposal, that you implemented a blockquote and alerts. If you have time left, please implement it here aswell:
![blockquote](/images/posts/blockquote.png)
![alerts](/images/posts/alerts.png)

# Comment

Please indicate the files you added or edited. Please use a comment within the files you edited.

```
# for HTML
<!-- ft-adjustment: <your comment> --->
# for css
/* ft-adjustment: <your comment> */
```
