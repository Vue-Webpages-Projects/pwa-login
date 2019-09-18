<template>
    <b-container fluid>
        <b-row align-v="center" align-h="center" style="height: 100vh; padding-bottom: 50px" >
            <b-col sm="12" md="3" class="login">
                <h1 class="text-center">
                    Contato
                </h1>

                <b-form v-if="show" @submit="onSubmit">
                    <b-form-group
                        label-for="name"
                        >
                        <b-form-input
                            id="name"
                            v-model="form.name"
                            type="text"
                            required
                            placeholder="Name"
                            ></b-form-input>
                    </b-form-group>

                    <b-form-group
                        label-for="email"
                        >
                        <b-form-input
                            id="email"
                            v-model="form.email"
                            type="email"
                            required
                            placeholder="Email"
                            ></b-form-input>
                    </b-form-group>

                    <b-form-textarea
                    id="message"
                    v-model="text"
                    placeholder="Message"
                    rows="3"
                    ></b-form-textarea>

                    <br>

                    <b-form-textarea
                    id="textarea"
                    v-model="text"
                    placeholder="Any suggestion?"
                    rows="2"
                    ></b-form-textarea>

                    <br>

                    
                    <div class="text-center">
                        <b-button type="submit" class="btn-block" variant="primary" style="margin-bottom: 10px">SEND</b-button>
                    </div>
                    
                </b-form>
            </b-col>
        </b-row>

        <navbar />
    </b-container>
</template>

<script>
import Navbar from '../components/Navbar'
export default {
    name: 'Contato',
    data() {
        return {
            form: {
                name: '',
                email: '',
                message: '',
                suggestion: ''
            },
            show: true
        }
    },
    methods: {
        onSubmit() {
            this.$router.push("/home")
        }
    },
    components: {
        Navbar
    }
}
</script>

<style scoped>
.login {
    padding: 15px 20px;
    margin: 20px;
    background-color: aliceblue;
    border-radius: 10px;
}

</style>