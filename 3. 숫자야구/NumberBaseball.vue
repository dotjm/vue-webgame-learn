//자바스크립트 파일로 생각할 것
<template>
    <div>
        <h1>{{result}}</h1>
        <form b-on:submit="onSubmitForm">
            <input ref="answer" maxlength="4" v-model="value">
            <button>입력</button>
        </form>
        <div>시도: {{}}</div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                value: '',
                result: '',
            }
        }, 
        methods: {
            onSubmitForm(e) {
                e.preentDefault();
            }
        }
    };
</script>

<style>

</style>