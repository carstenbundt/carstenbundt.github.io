---
layout: post
published: true 

comments: true

title: How to embed pdf on your Jekyll website
categories: website 

<!--
subtitle: 1 line of code (html)
[data science, website, html, pdf]
lead: 
-->

---
<!--
![Markdown](https://img.shields.io/badge/markdown-%23000000.svg?style=plastic&logo=markdown&logoColor=white) ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=plastic&logo=html5&logoColor=white)
-->

## Background
During the creation of this website, I struggled a little to figure out how to embed my CV in pdf. In the following I explain the steps I took to solve this issue. 

## Implementation
1. The first step is to create a folder (<mark>MYFOLDER</mark> in the code below) and upload the relevant pdf file (<mark>MYPDF.pdf</mark> in the code below). Note that you could also just directly upload your pdf in the main directory, but subdirectories will help to keep organized.
  
2. The second step is to create a separate page for your website where you want to display your pdf.

3. On this newly created page you enter the code below to embed the actual pdf. 

```html
---
layout: page
---

<object data="{{ site.url }}{{ site.baseurl }}/MYFOLDER/MYPDF.pdf" width="750" height="1000" type="application/pdf"></object> 

```

## Conclusion
Embedding a pdf on your Github-based website is easy and straightforward.

## Source
<a href="https://stackoverflow.com/questions/62206911/jekyll-gh-pages-embed-pdf">https://stackoverflow.com/questions/62206911/jekyll-gh-pages-embed-pdf</a>

