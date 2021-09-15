<template>
    <header class="position-absolute w-100">
        <Contacts />
        <Nav />
    </header>
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