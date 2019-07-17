<template>
    <div class="contents">
        <div class="contents-body">

            <h1>{{questions.name}}ファンクラブ</h1>
            <hr>
            <table bgcolor="#FFFFFF" border="0" cellpadding="0" cellspacing="0" class="board-form-table">
                <tr>
                    <td class="left tx14px" width="100">投稿者</td>
                    <td class="left" width="500">
                        <input id="textfield" name="textfield" type="text">
                    </td>
                </tr>
                <tr>
                    <td class="left tx14px" width="100">メールアドレス</td>
                    <td class="left" width="500">
                        <input id="textfield" name="textfield" type="text">
                    </td>
                </tr>
                <tr>
                    <td class="left tx14px" width="100">題名</td>
                    <td class="left" width="500">
                        <input id="textfield" name="textfield" type="text">
                    </td>
                </tr>
                <tr>
                    <td class="left tx14px vertical-align-top" width="100">コメント</td>
                    <td class="left top" width="500">
                        <textarea cols="45" id="textarea" name="textarea" rows="5"></textarea>
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td class="left top" width="500">
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
                <table bgcolor="#CCCCCC" border="0" cellpadding="0" cellspacing="1" width="600">
                    <tr>
                        <td>
                            <table
                                    style="background-color:#FFFFFF;padding-left:10px;padding-right:10px;padding-top:10px"
                                    width="600"
                            >
                                <tr>
                                    <td width="600">
                                        <span class="style7">はじめまして</span>
                                        <span class="tx14px">ハヤシ ( 2009/11/20 17:15 )</span>
                                    </td>
                                </tr>
                                <tr>
                                    <td class="tx14px">
                                        <span>こんな掲示板があるなんて知りませんでした！</span>
                                        <span>{{questions.name}}さんを応援する仲間ができて嬉しいです。{{questions.name}}ファン歴半年ですがよろしくおねがいします。</span>
                                    </td>
                                </tr>
                                <tr>
                                    <td class="tx14px">
                                        <hr size="1" style="color:#CCCCCC">
                                    </td>
                                </tr>
                                <tr>
                                    <td class="tx14px">
                                        <span class="style7">Re:はじめまして</span>chappie ( 2009/11/21 10:44 )
                                    </td>
                                </tr>
                                <tr>
                                    <td class="tx14px">ようこそ！
                                        {{questions.name}}さんを追ってもう2年になりますが心の中の炎は衰えません。こちらこそよろしくおねがいします。
                                    </td>
                                </tr>
                                <tr>
                                    <td class="tx14px">
                                        <hr size="1" style="color:#CCCCCC">
                                    </td>
                                </tr>
                                <tr>
                                    <td class="tx14px">
                                        <span class="style7">Re:Re:はじめまして</span>ゴードン ( 2009/11/21 14:51 )
                                    </td>
                                </tr>
                                <tr>
                                    <td class="tx14px">
                                        {{questions.name}}さんとはときどき会うことがありますが、とても魅力的なかたです
                                        <br>
                                    </td>
                                </tr>
                                <tr>
                                    <td class="tx14px">
                                        <hr size="1" style="color:#CCCCCC">
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
                                        <hr size="1" style="color:#CCCCCC">
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
                                        <hr size="1" style="color:#CCCCCC">
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
                        </td>
                    </tr>
                </table>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        props: {
            questions: Object
        }
    };
</script>

<style scoped>
    body {
        background-color: #ff9900;
        margin-top: 0px;
        margin-bottom: 0px;
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

    .orange {
        color: #ff6600;
        font-size: 12px;
        line-height: 148%;
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
    }

    .vertical-align-top {
        vertical-align: top;
    }

</style>