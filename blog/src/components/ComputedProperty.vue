<template>
<div>
    <h1>Computed Property</h1>
    <p>{{ (chocoChips*chocoChipsPrice) + (coldrink*coldrinkPrice) }}</p>
    <p>{{ (chocoChips*chocoChipsPrice) + (coldrink*coldrinkPrice) }}</p>

    <!-- this is the computed property -->
    <p>{{ totalPrice }}</p>

</div>
</template>

<script>
export default {
    name: "ComputedProperty",
    data() {
        return {
            chocoChips: 2,
            chocoChipsPrice: 10,
            coldrink: 1,
            coldrinkPrice: 20
        }
    },
    computed: {
        totalPrice() {
            return (this.chocoChips * this.chocoChipsPrice) + (this.coldrink * this.coldrinkPrice)
        }
    }

}
</script>
