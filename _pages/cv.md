---
# layout: cv
layout: none
permalink: /cv/
title: CV
nav: true
nav_order: 4
# cv_pdf: example_pdf.pdf # you can also use external links here
# description: This is a description of the page. You can modify it in '_pages/cv.md'. You can also change or remove the top pdf download button.
# toc:
#   sidebar: left
---

<!-- JS 优先跳转 -->
<script>
  window.location.replace('{{ "/assets/pdf/example_pdf.pdf" | relative_url }}');
</script>

<!-- Meta 兜底跳转 -->
<meta http-equiv="refresh" content="0; url={{ "/assets/pdf/example_pdf.pdf" | relative_url }}" />

<p>If you are not redirected, <a href="{{ "/assets/pdf/example_pdf.pdf" | relative_url }}">click here to open the CV (PDF)</a>.</p>