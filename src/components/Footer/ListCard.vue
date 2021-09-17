<template>
    <div class="list_card col-3">
        <div class="brand_color_base h-100 ps-5 py-4 rounded-3">
            <h2 class="color_white_txt mb-4 lh-sm">{{item.title}}</h2>
            <ul>
                <li class="my-2"  v-for="(element, index) in item.elements" :key="index"> {{element}} </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
  name: 'ListCard',
  props: ['item'],
}
</script>

<style lang="scss">
.list_card {
    ul {
        list-style-type: '> ';
        list-style-position: inside;
        li {
            display: revert;
        }
    }
}
</style>