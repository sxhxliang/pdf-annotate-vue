## pdf-annotate-vue

>  Annotation layer for pdf.js in vue


## Install

```
npm install pdf-annotate-vue -S
or
yarn add pdf-annotate-vue -S
```

## Example

```vue
<template>
  <div id="app">
     pdf path: {{pdf}}
    <pdfAnnotate :src="pdf" :toolbar="toolbar" :commentWrapper="commentWrapper"></pdfAnnotate>
  </div>
</template>

<script>

import pdfAnnotate from 'pdf-annotate-vue'
import "pdf-annotate-vue/src/css/toolbar.css";
import "pdf-annotate-vue/src/css/pdf_viewer.css";

export default {
  name: 'home',
  components: {
    pdfAnnotate
  },
  data(){
    return {
      pdf: './static/output.pdf',
      toolbar: true,
      commentWrapper: true,
    }
  }
}
</script>

```


## run example

```bash
# Clone Project
git clone https://github.com/AaronLeong/pdf-annotate-vue.git

cd pdf-annotate-vue/example
# Project setup --> install node_modules
yarn install
# Compiles and hot-reloads for development
yarn run serve

```