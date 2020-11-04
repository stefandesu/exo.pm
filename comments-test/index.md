---
title: comments test
layout: page
date: 2020-11-04 17:16:00
---

Testing comments via "Commento" here:

<script defer
  src="https://commento.exo.pm/js/commento.js"
  data-css-override="https://exo.pm/comments-test/commento-css.css">
</script>
<hr>
Note about comments: Currently, I only allow anonymous comments. Please check the "comment anonymously" box before adding a comment.
<div id="commento"></div>

Testing comments via "Isso" here:
<script data-isso="https://isso.exo.pm/"
        data-isso-reply-to-self="true"
        data-isso-max-comments-top="10"
        src="https://isso.exo.pm/js/embed.min.js">
</script>
<section id="isso-thread"></section>

<style>
#isso-thread .input-wrapper {
  font-size: 12px;
  margin-right: 2px;
}
#isso-thread .textarea:focus {
  color: black;
}
#isso-thread > h4 {
  color: #C9CACC;
}
#isso-thread input[name="email"], #isso-thread input[name="website"], #isso-thread input[name="preview"] {
  display: none;
}
</style>
