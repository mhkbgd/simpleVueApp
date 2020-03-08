<template>
    <div class="contact">
        
         FirstName : <input type = "text" v-model = "firstname" /> <br/><br/>
         LastName : <input type = "text" v-model = "lastname"/> <br/><br/>
         <h1>My name is {{firstname}} {{lastname}}</h1>
         <h1>Using computed method : {{getfullname}}</h1>
         <h1>Using method : {{namebymethod()}}</h1>
    </div>

</template>

<script>
export default {
    name: 'Contact',
    data: function(){
        return{
            message: "This is contact page",
            firstname: "",
            lastname: ""
        }
    },
    computed: {
        getfullname: function(){
            return this.firstname + " "+ this.lastname
        }
    },
    methods: {
        namebymethod: function(){
            return this.firstname+ " "+ this.lastname
        }
    }
}
</script>
<style lang="stylus" scoped>

</style>