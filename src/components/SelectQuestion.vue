<template>
    <div class="contents">
        <form @submit.prevent="handleSubmit" class="select-question tx12px">
            <p>step {{step}} / 6</p>
            <p>
                <label class="orange bold" for="name">{{message}}</label>
            </p>
            <template v-for="(choice, i) in choices">
                <div :key="choice">
                    <label>
                        <input :value="i+1" name="choice" type="radio" v-model="selectedValue">
                        <span>{{choice}}</span>
                    </label>
                </div>
            </template>
            <p>
                <button>次へ</button>
            </p>
        </form>
    </div>
</template>

<script>
    export default {
        props: {
            message: String,
            choices: Array,
            step: Number,
            value: Number
        },
        data() {
            return {
                advancedChoices: this.choices.map(c => c),
                selectedValue: this.value
            };
        },
        mounted() {
            // setInterval(() => {
            //   this.advancedChoices = this.advancedChoices.sort((a, b) =>
            //     Math.random() > 0.5 ? 1 : -1
            //   );
            //   console.log(this.advancedChoices);
            // }, 1000);
        },
        methods: {
            handleSubmit() {
                this.$emit("input", this.selectedValue);
                this.$emit("next");
            }
        }
    };
</script>

<style scoped>
    button {
        width: 60px;
    }

    .contents {
        width: 400px;
        margin: 0 auto;
        text-align: left;
    }

    .select-question {
        margin-bottom: 24px;
        padding-bottom: 24px;
        border-bottom: dotted 1px #c6c6c6;
    }

    .orange {
        color: #FF6600;
    }

    .bold {
        font-weight: bold;
    }

    .tx12px {
        font-size: 12px;
    }

</style>