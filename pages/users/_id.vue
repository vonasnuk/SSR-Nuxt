<template>
    <div>
        <section>
            <h1>User {{$route.params.id}}</h1>
        </section>
    </div>
</template>

<script>
    export default{
        validate({params}){
            return /^\d+$/.test(params.id)
        }
    }

</script>