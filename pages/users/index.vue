<template>
    <div>
        <section>
            <h1>Users</h1>
            <ul class="list-group">
                <li 
                class="list-group-item"
                v-for="user in users" :key='user.id'
                >
                    <a @click.prevent="openUser(user)" href="#">User {{user.name}}</a>
                </li>
            </ul>
        </section>
    </div>
</template>

<script>
export default{
    async asyncData({$axios}){
        const users = await $axios.$get('https://jsonplaceholder.typicode.com/users')
        return {users}
    },
    data(){
        return{
            users: []
        }
    },
    methods: {
        openUser(user) {
            this.$router.push('/users/' + user)
        }
    }
}
</script>