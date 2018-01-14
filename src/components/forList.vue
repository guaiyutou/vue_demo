<template>
    <div>
        <ul class="list">
            <li v-for='item in forItem'>
               <template>
                    <span v-for='(value, key, index) in item'>{{value}}----{{key}}------{{index}}</span>
                </template>
            </li>
        </ul>
        <ol class="list">
            <li v-for='(value, key, index) in obj'>
                {{value}}----{{key}}------{{index}}
            </li>
        </ol>
        <h3>多选按钮绑定一个值</h3>
        <input type="checkbox" id="isTrue" v-model='isTrue'>
        <label for="isTrue">{{isTrue}}</label>     
    </div>
</template>

<script type='text/javascript'>
    export default{
        name: 'forList',
        data () {
            return {
                forItem: [
                    {'name': 'yutou'},
                    {'name': 'chenlin'},
                    {'name': 'lili'}
                ],
                obj: {
                    firstName: 'JOND',
                    LastName: 'ddg',
                    age: 30
                },
                isTrue: true
            };
        }
    };
</script>