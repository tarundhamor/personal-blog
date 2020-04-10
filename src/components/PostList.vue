<template>
  <div class="post-list">
    <hr class="line" />
    <p class="date" v-html="post.date" />
    <h3 class="title" v-html="post.title" />
    <p class="description" v-html="post.description" />
    <b>{{post.timeToRead}} min read</b> &nbsp;
    <g-link :to="post.path" class="read">
      Read More
      <span class="visuallyhidden">about {{post.title}}</span>
    </g-link>
  </div>
</template>

<script>
export default {
  props: ["post"]
};
</script>

<style>
.line {
  border: 0.5px solid #cdc8c5;
  margin: 25px 0 30px;
}

.date {
  font-weight: 300;
}

.read {
  padding: 4px;
  color: #00ffa5;
  text-decoration: underline;
  border: 0px solid #00ffa5;
}

.visuallyhidden {
  position: absolute !important;
  width: 1px;
  height: 1px;
  padding: 0;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  white-space: nowrap;
  clip-path: inset(50%);
  border: 0;
}
.visuallyhidden:focus {
  display: inline-block;
  padding: 15px 23px 14px;
  width: auto;
  height: auto;
  clip: auto;
  color: #ffffff;
  background-color: #000000;
  clip-path: unset;
}
</style>
