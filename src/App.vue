<template>
  <div id="app">
      <InputName @next="step++" key="start" v-if="step === 1" v-model="questions.name"/>
      <SelectQuestion
              :choices="[
        '目',
        '肌',
        '指',
        '髪',
      ]"
              :step="step"
              @next="step++"
              message="自分の体で自慢できるところはどこですか？"
              v-if="step === 2"
              v-model="questions.q1"
      />
      <SelectQuestion
              :choices="[
        '我慢づよさ',
        '寝付きのよさ',
        'ごはんを食べるスピード',
        '体の柔らかさ',
      ]"
              :step="step"
              @next="step++"
              message="これは人に負けないというところはどこですか？"
              v-if="step === 3"
              v-model="questions.q2"
      />
      <SelectQuestion
              :choices="[
        '小学生のころ、なにかで賞状もらった',
        '中学生までは成績良かった',
        'バイト先で評判が良くて社員にならないかと言われた',
        '高校の同級生の母親に受けがよかった',
      ]"
              :step="step"
              @next="step++"
              message="過去の栄光で当てはまる、もしくはいちばん近いものを選んでください"
              v-if="step === 4"
              v-model="questions.q3"
      />
      <SelectQuestion
              :choices="[
        '嘘をつく',
        '金にきたない',
        '快楽におぼれる',
        '生意気だ',
      ]"
              :step="step"
              @next="step++"
              message="自分の欠点だと思うものはなんですか"
              v-if="step === 5"
              v-model="questions.q4"
      />
      <SelectQuestion
              :choices="[
        '濃い顔だ',
        '目が離れている',
        'まゆ毛がしっかりしている',
        'シュッとしている',
      ]"
              :step="step"
              @next="step++"
              message="あなたの顔の特徴でいちばん近いものを選んでください"
              v-if="step === 6"
              v-model="questions.q5"
      />
      <Result :questions="questions" v-if="step > 6"/>
  </div>
</template>

<script>
    import InputName from "./components/InputName.vue";
    import SelectQuestion from "./components/SelectQuestion.vue";
    import Result from "./components/Result.vue";

    export default {
        name: "app",
        data() {
            return {
                step: 1,
                questions: {
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

<style>
#app {
    font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
