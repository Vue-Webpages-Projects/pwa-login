<template>
    <b-container fluid>
        <b-row align-v="center" align-h="center" style="height: 100vh">
            <b-col sm="12" md="3" class="login">
                <h1 class="text-center">Login</h1>

                <b-form v-if="show">
                    <b-form-group
                        id="emailLogin"
                        label-for="email"
                        description="ex. email@email.com"
                        >
                        <b-form-input
                            id="email"
                            v-model="login.email"
                            type="email"
                            required
                            placeholder="Login or email"
                            ></b-form-input>
                    </b-form-group>

                    <b-form-group
                        id="passwordLogin"
                        label-for="password"
                        >
                        <b-form-input
                            id="password"
                            v-model="login.password"
                            type="password"
                            required
                            placeholder="Password"
                            ></b-form-input>
                    </b-form-group>

                    
                    <div class="text-center">
                        <b-button class="btn-block" style="margin-bottom: 10px">Login</b-button>
                        <router-link to="register">register</router-link>
                    </div>
                    
                </b-form>
            </b-col>
        </b-row>
    </b-container>
</template>

<script>
export default {
    name: 'Login',
    data() {
        return {
            login: {
                email: '',
                password: ''
            },
            show: true
        }
    }
}
</script>

<style scoped>
.login {
    padding: 20px;
    background-color: aliceblue;
    border-radius: 10px;
}
</style>