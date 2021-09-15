<template>
  <div class="demo">
    <input v-model='message' placeholder='edit me'>
    <p>Message is:{{message}}</p>
    
    <textarea v-model='message1' placeholder='content'></textarea>
    <span>Message is:</span>
    <p style="white-space:pre-line;">{{message1}}</p>

    <input type="checkbox" id="checkbox" v-model="checked">
    <label for="checkbox">{{checked}}</label>
  </div>
</template>

<script>
export default {
    data(){
        return {
            message:'',
            messag1:'',
            checked:'false',
        };
    },
    
}
</script>

<style>
 .demo{
     display:flex;
    text-align: start;
 }
 input{
     margin-right: 10px;
 }
</style>