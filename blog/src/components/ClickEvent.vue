<template>
<div>
    <h1> Click Event</h1>

    <div>
        <button v-on:click="clickEvent('Clicked')">Click Me</button>
        <p>{{ message }}</p>
    </div>
    <button v-on:dblclick="dblClick('Double Clicked')">Double Click</button>
    <button v-on:mousemove="MouseMove()">Mouse Move</button>
    <div>
        <button v-on:click="IncreaseCount()">Increase Count {{ count }}</button>
    </div>

</div>
</template>

<script>
export default {
    name: 'ClickEvent',
    data() {
        return {
            message: "Make me clicked",
            count : 0
        }
    },
    methods: {
        clickEvent(data) {
            this.message = data
        },
        dblClick(data) {
            alert(data)
        },
        MouseMove() {
            console.log("Mouse is moving")
        },
        IncreaseCount(){
            this.count++
        }

    }
}
</script>
