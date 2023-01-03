<template>
    <form action="">
        <div><InputTextForm/></div>
        <div> <InputTextForm/></div>
       <div><SubmitForm/></div>
        
    </form>
</template>

<script>
import InputTextForm from './form/InputTextForm.vue';
import SubmitForm from './form/SubmitForm.vue';
export default{
    name: 'FormComponente',
    components:{
        InputTextForm,
        SubmitForm
    }
}
</script>