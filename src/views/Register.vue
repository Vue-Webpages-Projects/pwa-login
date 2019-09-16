<template>
    <b-container fluid >
        <b-row align-v="center" align-h="center" style="height: 100vh" >
            <b-col sm="12" md="4" class="login">
                <h1 class="text-center">Register</h1><br>

                <b-form v-if="show" @submit="onSubmit">
                    <b-row>
                        <b-col sm="12" md="6">
                            <b-form-group
                                id="usernameUser"
                                label-for="user"
                                >
                                <b-form-input
                                    id="user"
                                    v-model="login.username"
                                    type="text"
                                    required
                                    placeholder="Username"
                                    ></b-form-input>
                            </b-form-group>
                        </b-col>

                        <b-col sm="12" md="6">
                            <b-form-group
                                id="numeroContato"
                                label-for="contato"
                                >
                                <b-form-input
                                    id="contato"
                                    v-model="login.contato"
                                    type="number"
                                    placeholder="Phone"
                                    ></b-form-input>
                            </b-form-group>
                        </b-col>

                        <b-col sm="12">
                            <b-form-group
                                id="emailEmail"
                                label-for="email"
                                >
                                <b-form-input
                                    id="email"
                                    v-model="login.email"
                                    type="email"
                                    required
                                    placeholder="Email"
                                    ></b-form-input>
                            </b-form-group>
                        </b-col>
                    

                        <b-col sm="12">
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
                        </b-col>

                        <b-col sm="12">
                            <b-form-group
                                id="passwordLogin"
                                label-for="password"
                                >
                                <b-form-input
                                    id="password"
                                    v-model="login.password"
                                    type="password"
                                    required
                                    placeholder="Confirm password"
                                    ></b-form-input>
                            </b-form-group>
                        </b-col>
                    </b-row>

                    <div class="text-center">
                        <b-button type="submit" class="btn-block" variant="primary" style="margin-bottom: 10px">Register</b-button>
                        <router-link to="/">Login</router-link>
                    </div>

                </b-form>
            </b-col>
        </b-row>
    </b-container>
</template>

<script>
export default {
    name: 'Register',
    data() {
        return {
            login: {
                email: '',
                contato: '',
                username: '',
                password: '',
                confirmation: ''
            },
            show: true
        }
    },
    methods: {
        onSubmit() {
            this.$router.push("/home")
        }
    }
}
</script>

<style scoped>
.login {
    padding: 20px;
    margin: 20px;
    background-color: aliceblue;
    border-radius: 10px;
}
</style>