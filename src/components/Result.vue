<template>
    <div class="contents">
        <div class="contents-body">

            <h1>{{choiceQuestions.name}}ファンクラブ</h1>
            <hr>
            <table class="board-form-table">
                <tr>
                    <td class="form-label">投稿者</td>
                    <td class="form-right">
                        <label>
                            <input type="text">
                        </label>
                    </td>
                </tr>
                <tr>
                    <td class="form-label">メールアドレス</td>
                    <td class="form-right">
                        <label>
                            <input type="text">
                        </label>
                    </td>
                </tr>
                <tr>
                    <td class="form-label">題名</td>
                    <td class="form-right">
                        <label>
                            <input type="text">
                        </label>
                    </td>
                </tr>
                <tr>
                    <td class="form-label vertical-align-top">コメント</td>
                    <td class="form-right">
                        <label>
                            <textarea cols="45" rows="5"></textarea>
                        </label>
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td class="form-right">
                        <span class="tx12px">現在、ファン殺到中につき書き込みを一時中止しています</span>
                    </td>
                </tr>
            </table>

            <div class="contents__header left">
                <hr>
                <em class="tx14px">新着の記事10件を表示しています。</em>
                <hr>
            </div>

            <div class="contents__board left">
                <table class="board-output-table">
                    <tr>
                        <td>
                            <span class="style7">はじめまして</span>
                            <span class="tx14px">ハヤシ ( 2009/11/20 17:15 )</span>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span>こんな掲示板があるなんて知りませんでした！</span>
                            <span>{{choiceQuestions.name}}さんを応援する仲間ができて嬉しいです。{{choiceQuestions.name}}ファン歴半年ですがよろしくおねがいします。</span>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <hr>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span class="style7">Re:はじめまして</span>chappie ( 2009/11/21 10:44 )
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">ようこそ！
                            {{choiceQuestions.name}}さんを追ってもう2年になりますが心の中の炎は衰えません。こちらこそよろしくおねがいします。
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <hr>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span class="style7">Re:Re:はじめまして</span>ゴードン ( 2009/11/21 14:51 )
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            {{choiceQuestions.name}}さんとはときどき会うことがありますが、とても魅力的なかたです
                            <br>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <hr>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span class="style7">Re:Re:Re:はじめまして</span>ハヤシ ( 2009/11/21 19:22)
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            うらやましー！ どんな匂いがしますか？
                            <br>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <hr>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span class="style7">Re:Re:Re:Re:はじめまして</span>ゴードン ( 2009/11/21 23:17 )
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">レコードクリーナーのスプレーみたいな匂いがしますよ。</td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <hr>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span class="style7">Re:Re:Re:Re:Re:はじめまして</span>ハヤシ ( 2009/11/22 9:49 )
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">さっそくレコードクリーナーを買ってきます♪</td>
                    </tr>
                </table>

                <table class="board-output-table">
                    <tr>
                        <td>
                            <span class="style7">やっぱり{{questions.q1.select[choiceQuestions.q1 - 1]}}ですよね</span>
                            <span class="tx14px">谷P ( 2009/11/18 23:56 )</span>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span>{{choiceQuestions.name}}様の魅力は{{questions.q1.select[choiceQuestions.q1 - 1]}}ですよね。こっそり見ているとつくづくそう思います。</span>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <hr>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span class="style7">そうそう！</span>u-chan ( 2009/11/18 23:59 )
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span>あの美しい{{questions.q1.select[choiceQuestions.q1 - 1]}}はそうそうあるもんじゃないですよね。同性の私が言うのもなんですが。</span>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <hr>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span class="style7">Re:そうそう！</span>ロベルト ( 2009/11/19 1:21 )
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span>
                                わたしは内面からにじみ出る細やかさも見逃せないと思います。繊細さというか。(^o^)
                            </span>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <hr>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span class="style7">なるほどー</span>阿Q ( 2009/11/19 4:53)
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span>
                                一見そうは思わせないけど繊細なところがありますよね。それが{{questions.q1.select[choiceQuestions.q1 - 1]}}に現れているのではないでしょうか。
                            </span>
                        </td>
                    </tr>
                </table>

                <table class="board-output-table">
                    <tr>
                        <td>
                            <span class="style7">{{choiceQuestions.name}}様のいいところ！</span>
                            <span class="tx14px">ボーキサイト ( 2009/11/10 5:45 )</span>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span>なんと言っても{{questions.q2.select[choiceQuestions.q2 - 1]}}だと思います。</span>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <hr>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span class="style7">賛成！</span>活断層 ( 2009/11/12 8:16 )
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span>それはありますねー。{{choiceQuestions.name}}様の{{questions.q2.select[choiceQuestions.q2 - 1]}}は国体クラスなんじゃないかと思います。</span>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <hr>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span class="style7">新情報</span>サハリン ( 2009/11/12 10:11 )
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span>
                                噂によると、学生時代「{{questions.q2.select[choiceQuestions.q2 - 1]}}オブザイヤー」に選ばれたらしいですよ。幼なじみだという人に聞きました。
                            </span>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <hr>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span class="style7">Re:新情報</span>るな ( 2009/11/15 20:35)
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span>
                                わたしも憧れて{{questions.q2.select[choiceQuestions.q2 - 1]}}を訓練しているのですが、なかなかあのレベルにまでは行きません。
                            </span>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <hr>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span class="style7">Re:Re:新情報</span>太郎 ( 2009/11/15 20:46)
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span>
                                無理すると体をこわすかもしれないから気をつけて！
                            </span>
                        </td>
                    </tr>
                </table>

                <table class="board-output-table">
                    <tr>
                        <td>
                            <span class="style7">{{choiceQuestions.name}}トリビア</span>
                            <span class="tx14px">マグマ ( 2009/11/17 3:16 )</span>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span>聞いた話では{{questions.q3.select[choiceQuestions.q3 - 1]}}らしいですよ。</span>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <hr>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span class="style7">Re:{{choiceQuestions.name}}トリビア</span>アムンゼン ( 2009/11/18 11:45 )
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span>
                                すごいですね！激レア情報ありがとうございます
                            </span>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <hr>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span class="style7">Re:Re:{{choiceQuestions.name}}トリビア</span>パナマ運河庁 ( 2009/11/19 11:33 )
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span>
                                ますますファンになってしまいました
                            </span>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <hr>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span class="style7">たぶん…</span>蒲田子 ( 2009/11/19 12:45)
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span>
                                {{choiceQuestions.name}}っちが保険のセールスマンやっていたらきっとトップセールスだと思います。
                            </span>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <hr>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span class="style7">Re:たぶん…</span>土偶 ( 2009/11/19 13:01)
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span>
                                その感じすごくわかります～
                            </span>
                        </td>
                    </tr>
                </table>

                <table class="board-output-table">
                    <tr>
                        <td>
                            <span class="style7">激安情報</span>
                            <span class="tx14px">林雄司 ( 2009/11/25 2:10 )</span>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span>
                                「デイリーポータルZのなんか売る場所」ではここでしか買えないグッズを販売中。絶対得だからクリックしてみて！<br/>
                                <a href="https://dailyportalz.booth.pm/">https://dailyportalz.booth.pm/</a>
                            </span>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <hr>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span class="style7">なにこれ</span>ポッキー ( 2009/11/25 3:44 )
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span>
                                宣伝ですよね。これw
                            </span>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <hr>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span class="style7">Re:なにこれ</span>林雄司 ( 2009/11/26 4:21 )
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span>
                                デイリーポータルZをはげます会もヨロシク<br/>
                                <a href="https://dailyportalz.jp/hagemasu_goannai">https://dailyportalz.jp/hagemasu_goannai</a>
                            </span>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <hr>
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span class="style7">Re:Re:なにこれ</span>イカ子( 2009/11/26 8:01)
                        </td>
                    </tr>
                    <tr>
                        <td class="tx14px">
                            <span>
                                空気よんでほしいですよねー。管理人さん、削除しなくていいんですか？
                            </span>
                        </td>
                    </tr>
                </table>

            </div>
        </div>
    </div>
</template>

<script>
    import questions from '../mixins/Questions';

    export default {
        mixins: [questions],
        props: {
            choiceQuestions: Object
        }
    };
</script>

<style lang="scss" scoped>
    body {
        background-color: #ff9900;
        margin-top: 0;
        margin-bottom: 0;
    }

    td {
        padding: 0;
    }

    .tx14px {
        font-size: 14px;
        line-height: 144%;
    }

    .contents {
        width: 800px;
        margin: 0 auto;
    }

    .contents-body {
        width: 600px;
        margin: 0 auto;
    }

    .left {
        text-align: left;
    }

    .top {
        vertical-align: top;
    }

    .contents__header {
        margin: 30px 0;
    }

    .tx12px {
        font-size: 12px;
        line-height: 160%;
    }

    .style7 {
        color: #400040;
        font-size: 14px;
        font-weight: bold;
        margin-right: 6px;
    }

    .board-form-table {
        width: 620px;
        margin: 0 auto;
        border-collapse: collapse;
    }

    .board-output-table {
        width: 600px;
        border-collapse: separate;
        border: 1px #CCCCCC solid;
        border-spacing: 1px;
        padding: 10px;
        margin: 0 auto 50px;
    }

    .vertical-align-top {
        vertical-align: top;
    }

    .form-label {
        @extend .left;
        @extend .tx14px;
        width: 100px;
    }

    .form-right {
        @extend .left;
        width: 500px;
    }


</style>