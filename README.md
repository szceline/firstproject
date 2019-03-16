<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>
<body>
    <div id="app">
        <p>{{message}}</p>
        <button v-on:click="changeMethod">点击按钮</button>
    </div>

    <script src="vue.js"></script>

    <script>
         new Vue({
            el: '#app' ,
            data :{
                message :'hello vue!'
            },
            methods:{
                changeMethod:function(){
                    this.message ="hi vue.js";
                }
            }
        });
    </script>
</body>
</html>
