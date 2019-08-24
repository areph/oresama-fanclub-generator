<template>
    <div id="app">
        <InputName @next="step++" key="start" v-if="step === 1" v-model="choiceQuestions.name"/>
        <SelectQuestion
                :choices="questions.q1.select"
                :step="step"
                @next="step++"
                message="自分の体で自慢できるところはどこですか？"
                v-if="step === 2"
                v-model="choiceQuestions.q1"
        />
        <SelectQuestion
                :choices="questions.q2.select"
                :step="step"
                @next="step++"
                message="これは人に負けないというところはどこですか？"
                v-if="step === 3"
                v-model="choiceQuestions.q2"
        />
        <SelectQuestion
                :choices="questions.q3.select"
                :step="step"
                @next="step++"
                message="過去の栄光で当てはまる、もしくはいちばん近いものを選んでください"
                v-if="step === 4"
                v-model="choiceQuestions.q3"
        />
        <SelectQuestion
                :choices="questions.q4.select"
                :step="step"
                @next="step++"
                message="自分の欠点だと思うものはなんですか"
                v-if="step === 5"
                v-model="choiceQuestions.q4"
        />
        <SelectQuestion
                :choices="questions.q5.select"
                :step="step"
                @next="step++"
                message="あなたの顔の特徴でいちばん近いものを選んでください"
                v-if="step === 6"
                v-model="choiceQuestions.q5"
        />
        <Result :choiceQuestions="choiceQuestions" v-if="step > 6"/>
    </div>
</template>

<script>
    import InputName from "./components/InputName.vue";
    import SelectQuestion from "./components/SelectQuestion.vue";
    import Result from "./components/Result.vue";
    import questions from './mixins/Questions';

    export default {
        name: "app",
        mixins: [questions],
        data() {
            return {
                step: 1,
                choiceQuestions: {
                    name: "",
                    q1: 1,
                    q2: 1,
                    q3: 1,
                    q4: 1,
                    q5: 1
                }
            };
        },
        methods: {},
        components: {
            InputName,
            SelectQuestion,
            Result
        }
    };
</script>

<style lang="scss">
    #app {
        font-family: "Avenir", Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }
</style>
