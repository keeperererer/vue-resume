<template>
  <div id="app">
    <ShowMenu v-on:listenShowMenu='listenShowMenu'></ShowMenu>
    <!-- <ShowStyle ref="comShowStyle"></ShowStyle>
    <ShowResume ref="comShowResume" :resumeData="resumeData"></ShowResume>
    <transition name="fade">
        <FormList 
        ref="comFormList" 
        :resumeData="resumeData" 
        v-if="formListShow"
        v-on:listenFormList='listenFormList'>
        </FormList>
    </transition> -->
  </div>
</template>

<script>
import ShowMenu from './components/showMenu/showMenu.vue'

export default {
  name: 'App',
  components: {
    ShowMenu
  }
}
</script>

<style>
import 
    /* 内外边距通常让各个浏览器样式的表现位置不同 */
    body, div, dl, dt, dd, ul, ol, li, h1, h2, h3, h4, h5,
    h6, pre, code, form, fieldset, legend, input, textarea,
    p, blockquote, th, td, hr, button, article, aside, details,
    figcaption, figure, footer, header, menu, nav, section {
        margin: 0;
        padding: 0;
    }

    input, select, textarea {
        font-size: 100%;
    }

    input {
        outline: none;
        border-style: none
    }

    /* 去掉各 Table  cell 的边距并让其边重合 */
    table {
        border-collapse: collapse;
        border-spacing: 0;
    }

    /* 去除默认边框 */
    fieldset, img {
        border: 0;
    }

    /* 去掉 firefox 下此元素的边框 */
    abbr, acronym {
        border: 0;
        font-variant: normal;
    }

    /* 一致的 del 样式 */
    del {
        text-decoration: line-through;
    }

    address, caption, cite, code, dfn, em, th, var {
        font-style: normal;
        font-weight: 500;
    }

    /* 去掉列表前的标识, li 会继承 */
    ol, ul {
        list-style: none;
    }

    /* 对齐是排版最重要的因素, 别让什么都居中 */
    caption, th {
        text-align: left;
    }

    a {
        text-decoration: none;
    }

    /*清除浮动代码*/
    .clearfloat:after {
        display: block;
        clear: both;
        content: "";
        visibility: hidden;
        height: 0
    }

    .clearfloat {
        zoom: 1
    }

    body, html {
        width: 100%;
        height: 100%;
        padding: 0;
        margin: 0;
        min-width: 1024px;
        font-size: 62.5%;
    }

    #app {
        width: 100%;
        height: 100%;
    }

    .fade-enter-active, .fade-leave-active {
        transition: opacity .5s
    }

    .fade-enter, .fade-leave-active {
        opacity: 0
    }
</style>

