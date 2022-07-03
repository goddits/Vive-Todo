<template>
  <div class="home">
    <div class="box-left">
      <!--example  -->
      <div class="example">
        <p>Vue.js</p>
        <div class="title">Example</div>
        <span>charles hong</span>
      </div>
      <!-- introduction -->
      <div class="introduction">
        <p class="text">
          Vue.js provides efficient MVVM data bindings with a simple and
          flexible API. It uses plain JavaScript object models, DOM-based
          templating and extendable directives and filters.
        </p>
        <div class="info"><a href="https://vuejs.org/">Vue.js</a></div>
      </div>
      <!-- Official -->
      <div class="official">
        <!-- resources -->
        <div class="resources">
          <h3>Official Resources</h3>
          <ul>
            <li>
              <a href="https://vuejs.org/guide/introduction.html"
                >Documentation</a
              >
            </li>
            <li><a href="https://vuejs.org/api/">API Reference</a></li>
            <li>
              <a href="https://vuejs.org/examples/#hello-world">Examples</a>
            </li>
            <li>
              <a href="https://github.com/vuejs/vue">Vue.js on GitHub</a>
            </li>
          </ul>
        </div>
        <!-- Community -->
        <div class="community">
          <h3>Community</h3>
          <ul>
            <li><a href="https://twitter.com/vuejs">Twitter</a></li>
            <li><a href="https://gitter.im/vuejs/vue">Gitter Channel</a></li>
            <li>
              <a href="https://github.com/vuejs/Discussion/issues"
                >Discussions on GitHub</a
              >
            </li>
          </ul>
        </div>
      </div>
      <div class="other">
        <p>
          If you have other helpful links to share, or find any of the links
          above no longer work, please let us know.
        </p>
      </div>
    </div>
    <div class="box-center">
      <h1>todos</h1>
      <input type="text" placeholder="What needs to be done ?" v-model="msg" />
    </div>
    <div class="box-right">
      <h3>Tools</h3>
      <ul>
        <li><a href="https://www.deepl.com" target="_blank">DeepL</a></li>
        <li>
          <a href="https://developer.mozilla.org" target="_blank"
            >Mdn web dos</a
          >
        </li>
        <li><a href="https://leetcode-cn.com/" target="_blank">leetcode</a></li>
        <li><a href=""></a></li>
        <li><a href=""></a></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Home',
  data() {
    return {
      msg: ''
    }
  }
}
</script>
<style lang="scss" scoped>
.home {
  display: flex;
  justify-content: center;
}
.box-left {
  width: 300px;
  margin-top: 10px;
  padding: 0 20px;
  .example {
    border-bottom: 2px dotted #ccc;
    padding-bottom: 10px;
    p {
      font-size: 20px;
      padding-bottom: 5px;
    }
    .title {
      font-size: 14px;
    }
  }
  .introduction {
    padding: 20px 0;
    position: relative;
    .text {
      background: #f1f2f3;
      font-size: 16px;
    }
    .info {
      position: absolute;
      right: 0;
    }
  }
  .official {
    border-top: 2px dotted #ccc;
    border-bottom: 2px dotted #ccc;
    margin-top: 10px;
    padding: 20px 0;
  }
  .other {
    padding: 20px 0;
  }
}
.box-center {
  height: 100vh;
  flex: 1;
  text-align: center;
  background: #f1f2f3;
}
.box-right {
  width: 200px;
  text-align: center;
}
</style>
