<template>
  <section class="prefooter">
    <div class="container">
      <ul class="icons-list">
        <li v-for="(item,index) in icons" :key="index">
          <img :src="require(`../assets/img/${item.img}`)" alt="" />
          <h3>{{ item.text }}</h3>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: "AppPrefooter",
  data: function() {
    return {
      icons: [
        {
          img: 'buy-comics-digital-comics.png',
          text: 'Digital Comics'
        },
        {
          img: 'buy-comics-merchandise.png',
          text: 'DC merchandise'
        },
        {
          img: 'buy-comics-subscriptions.png',
          text: 'Subscription'
        },
        {
          img: 'buy-comics-shop-locator.png',
          text: 'Comic shop locator'
        },
        {
          img: 'buy-dc-power-visa.svg',
          text: 'DC power visa'
        }
      ]
    }
  }
};
</script>

<style lang="scss" scoped>
.prefooter {
  background-color: blue;
  color: white;
  padding: 2rem 0;

  .icons-list {
    display: flex;

    li {
      width: calc(100% / 5);
      display: flex;
      align-items: center;
      padding: .5rem;

      img {
        width: 20%;
        margin-right: 1rem;
      }

      h3 {

      }
    }
  }
}
</style>