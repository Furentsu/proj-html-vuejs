<template>
  <div class="col-3">
      <h3>Contact Us Today</h3>

      <ul>
        <li v-for="(element,index) in contacts" :key="index">
            <div class="icon-container">
                <i :class="contacts[index].iconClass"></i>
            </div>

            <div class="content ">
                <span class="d-block">{{contacts[index].text}}</span>
                <span class="d-block">{{contacts[index].address}}</span>
                <span class="d-block">{{contacts[index].postCode}}</span>
            </div>
        </li>
      </ul>
  </div>
</template>

<script>
export default {
    name: 'FooterContacts',
    props: ['contacts']
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

ul {
    list-style: none;
    padding-left: 0;

    li {
        display: flex;
    }
}


</style>