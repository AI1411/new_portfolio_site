<template>
  <div class="columns is-mobile">
    <div class="column is-three-fifths is-offset-one-fifth">
      <div class="content is-medium">
        <h3 class="title is-3">直近の業務経歴</h3>
        <div class="box" v-for="item in items">
          <h4 class="title is-3">{{ item.company }}({{ item.period }})</h4>
          <article class="message is-primary">
            <div class="message-body">
              形態: {{ item.title }}<br><br>
              業務内容: {{ item.body }}<br>
              使用技術: {{  item.skill  }} <br>
              使用ツール： {{ item.tool }}<br>
              主な役割: {{  item.role }}<br>
              携わった機能: {{ item.about }}
            </div>
          </article>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from 'axios';
export default {
  data() {
    return {
      items: []
    }
  },
  async asyncData({ app, error}) {
    try {
      const {data} = await axios.get(
        "https://akira-portfolio.microcms.io/api/v1/contents", {
          headers: {"X-API-KEY": process.env.API_KEY}
        }
      );
      return {
        items: data.contents
      }
    } catch (err) {

    }
  }
}
</script>

<style scoped>
</style>
