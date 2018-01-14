<template>
    <div id="app">
        <bing/>
        <ForList/>
        <!-- <HelloWorld/> -->
    </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld';
import bing from './components/bing';
import ForList from './components/forList';

export default {
    name: 'app',
    components: {
        bing, ForList
    }
};
</script>

<style>
#app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    margin-top: 60px;
}
</style>
