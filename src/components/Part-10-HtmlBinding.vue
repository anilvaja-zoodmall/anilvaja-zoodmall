<template>
    <div>
        <h1>{{text}}</h1>
        <div v-html="tag">
        </div>
        <div v-html="tag2">
        </div>
    </div>
</template>
<script>
export default {
    name:'HtmlBinding',
    data(){
        return {
            text:"sampleText",
            tag:"<h1>Test</h1>",
            tag2:"<h1>anil.vaja@test.com</h1>",
        }
    }
}
</script>