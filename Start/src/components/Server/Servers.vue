<template>
    <div class="col-xs-12 col-sm-6">
        <ul class="list-group">
            <!-- <li
                    class="list-group-item"
                    v-for="index in 5">
                Server #{{ index }}
            </li> -->
            <li class="list-group-item"  v-for="server in servers"> <a href="#"> ID:{{ server.id }} Status:{{ server.status }}</a> </li>
        </ul>
    </div>
</template>

<script>

// import { busEvent } from '../main';

export default{
    data: function(){
        return{
            servers: [
                {id: 1, status: 'Critical'},
                {id: 2, status: 'Normal'},
                {id: 3, status: 'Unknown'},
                {id: 4, status: 'Normal'}
            ]
        }
    }
}
</script>

<style>

</style>
