---
layout: doc
---

<script setup>
  import {data assignments} from './assignments/assignments.data';
  import { withBase } from 'vitepress';
</script>

# Assignments

<ul v-if="blogs.length > 0">
  <li v-for="blog of blogs">
    <a :href="withBase(assignments.url)">{{ assignments.frontmatter.title }}</a>
  </li>
</ul>
<p v-else>
  Nothing here yet!
</p>
