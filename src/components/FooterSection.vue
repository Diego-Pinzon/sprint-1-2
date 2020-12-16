<template>
    <div id = "section-footer">
        <footer class="footer ">
            <div class="d-flex justify-content-center">
                <div class="col-md-2">
                    <h5 class="text-md-right">Contactenos</h5>
                    <hr>
                </div>
                <div class="col-md-5">
                    <form @submit.prevent="sendEmail">
                        <div class="form-group">
                            <input class="form-control" type="text" v-model="name" name="name"
                                placeholder="Ingrese su nombre">
                        </div>
                        <div class="form-group">
                            <input class="form-control" type="email" v-model="email" name="email"
                                placeholder="Ingrese su email">
                        </div>
                        <div class="form-group">
                            <textarea class="form-control" name="message" v-model="message" cols="30" rows="5"
                                placeholder="Message">
                            </textarea>
                        </div>
                        <div class="form-group text-xs-right">
                            <button type="submit" class="btn btn-primary" value="Send">Enviar</button>
                        </div>
                    </form>
                </div>
            </div>
            <div class="footer-copyright text-center py-3">© 2020 Copyright:
                <a href=""> SpaceX</a>
            </div>
        </footer>
        
    </div>
</template>

<script>
    import emailjs from 'emailjs-com'

    export default {
        name: 'ContactUs',
        data() {
            return {
                name: '',
                email: '',
                message: ''
            }
        },
        methods: {
            sendEmail(e) {
                try {
                    emailjs.sendForm('service_98j3trb', 'template_xll1dxp', e.target,
                        'user_cjyheEvO3I9xP9DDPA9Z9', {
                            name: this.name,
                            email: this.email,
                            message: this.message
                        })

                } catch (error) {
                    console.log({
                        error
                    })
                }
                // Reset form field
                this.name = ''
                this.email = ''
                this.message = ''
            },
        }
    }
</script>
