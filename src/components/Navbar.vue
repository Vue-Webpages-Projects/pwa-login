<template>

    <b-navbar type="dark" variant="dark" fixed="bottom" style="justify-content: center;">
        <b-navbar-nav >

            <router-link to="/home">
                <b-nav-item href="/home"><i class="fas fa-home" style="font-size: 25px; margin: auto 20px"></i></b-nav-item>
            </router-link>

            <router-link to="/index">
                <b-nav-item href="/content"><i class="fab fa-buromobelexperte" style="font-size: 25px; margin: auto 20px"></i></b-nav-item>
            </router-link>

            <router-link to="/about">
                <b-nav-item href="/about"><i class="fas fa-user" style="font-size: 25px; margin: auto 20px"></i></b-nav-item>
            </router-link>

            <router-link to="/contato">
                <b-nav-item href="/contact"><i class="fas fa-envelope" style="font-size: 25px; margin: auto 20px"></i></b-nav-item>
            </router-link>

        </b-navbar-nav>
    </b-navbar>
</template>

<script>
export default {
    name: 'Navbar'
}
</script>

<style scoped>

a:hover {
    text-decoration-line: none;
}

.navbar-drop *:hover{
    color: aliceblue!important;
}

.navbar-item {
    background-color: transparent!important;
    transition: .5s;

}
.navbar-item:hover {
    background-color: #2c3e50!important;
    color: white!important;
    transition: .5s;
}   

</style>