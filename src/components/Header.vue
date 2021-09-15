<template>
    <div>
        <Contacts />
        <Nav />
    </div>
</template>

<script>
import Contacts from "./Contacts.vue";
import Nav from "./Nav.vue";
export default {
    name: "Header",
    components: {
        Contacts,
        Nav,
    }
}
</script>

<style>

</style>