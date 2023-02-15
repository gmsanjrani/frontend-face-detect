<template>
    <div class="outer_input_container">
        <img class="wave" src="../assets/images/wave.png" />
        <div class="input_container">
            <div class="img">
                <img src="../assets/images/bg.svg" />
            </div>
            <div class="login_content">
                <form>
                    <img src="../assets/images/avatar.svg" />
                    <h2 class="title">Signup</h2>
                    <div class="input_input_container one">
                        <div class="icon">
                            <i class="fas fa-user"></i>
                        </div>
                        <div class="div">
                            <h5>Username</h5>
                            <input @focus="focus($event)" @blur="blur($event)"  type="text" class="input" />
                        </div>
                    </div>
                    <div class="input_input_container pass">
                        <div class="icon">
                            <i class="fas fa-lock"></i>
                        </div>
                        <div class="div">
                            <h5>Password</h5>
                            <input @focus="focus($event)" @blur="blur($event)" type="password" class="input" />
                        </div>
                    </div>
                    <div class="input_input_container pass">
                        <div class="icon">
                            <i class="fas fa-lock"></i>
                        </div>
                        <div class="div">
                            <h5>Confirm</h5>
                            <input @focus="focus($event)" @blur="blur($event)" type="password" class="input" />
                        </div>
                    </div>
                    <div class="signup_forget">
                        <p href="#">Already have an account?</p>
                        <a href="#">Login</a>
                    </div>
                    <input type="submit" class="btn" value="Signup" />
                </form>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "SignupPage",
    methods: {
        focus(e) {
            let parent = e.target.parentNode.parentNode;
            parent.classList.add("focus");
        },
        blur(e) {
            let parent = e.target.parentNode.parentNode;
            if (e.target.value == "") {
                parent.classList.remove("focus");
            }
        },
    },
};
</script>

<style scoped>
@import "../assets/login-signup";
</style>
