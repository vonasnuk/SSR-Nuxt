<template>
    <div>
        <section>
            <form>
                <h1>Login page</h1>
                <br>
                <div class="form-group row">
                    <label for="inputEmail3" class="col-sm-2 col-form-label">Email</label>
                    <div class="col-sm-10">
                    <input type="email" class="form-control" id="inputEmail3">
                    </div>
                </div>
                <div class="form-group row">
                    <label for="inputPassword3" class="col-sm-2 col-form-label">Password</label>
                    <div class="col-sm-10">
                    <input type="password" class="form-control" id="inputPassword3">
                    </div>
                </div>
                <p>
                    <nuxt-link to="/">To home page</nuxt-link>
                </p>
                <div class="form-group row">
                    <div class="col-sm-10">
                    <button type="submit" class="btn btn-primary">Sign in</button>
                    </div>
                </div>
                </form>
        </section>
    </div>
</template>
<script>
    export default {
        layout: 'first'
    }
</script>

<style scoped>
    form{
        width: 50%;
        display: block;
        margin: auto;
    }
</style>