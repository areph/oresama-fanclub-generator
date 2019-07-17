<template>
    <div class="contents">
        <form @submit.prevent="handleSubmit" class="input-question tx12px">
            <p>step 1 / 6</p>
            <label class="orange bold" for="name">名前を入れてください</label>
            <br>
            <input class="input-name" id="name" required type="text" v-model="name">
            <p>
                <button>次へ</button>
            </p>
        </form>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                name: ""
            };
        },
        methods: {
            handleSubmit() {
                this.$emit("input", this.name);
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

    .input-question {
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

    .input-name {
        width: 300px;
    }
</style>
