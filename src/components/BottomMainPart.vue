<template>
    <div class = "bottomcontainer">
        <div class = "bottomtoppart">
            <div>
            <p>No.of.rounds</p>
            <input class="countinputbox" type = "text" />
            <i class="fa fa-plus" aria-hidden="true"> </i>
            </div> 
            <div>
            <p>Type Of Rounds </p>
            <select >
                <option>Consecutive Rounds </option>
                <option>Parallel Rounds </option>
            </select>
            </div>
            <div>
            <p>Type Of Contest </p>
            <select>
                <option>Online/Offline Rounds</option>
                <option>Offline Contest</option>
                <option>Online Contest</option>
            </select>
            </div>
        
        
        </div>
        <hr class="line-through"/>
        <div class = "bottomlowerpart">
            <ListComponent />
            <Extra/>
        </div>
    </div>
</template>

<script>
import ListComponent from "./ListComponent.vue"
import Extra from "./Extra.vue"
   
export default {
    components:{
    ListComponent,
    Extra
    },
}
</script>

<style>
.bottomcontainer{
    display:flex;
    flex-direction:column;
}
.bottomtoppart{
    display:flex;
    flex-direction: row;
    justify-content: space-evenly;
}
.line-through{
    border:1px solid black;
    width:100%;
}
.bottomlowerpart{
    display:flex;
    justify-content: space-evenly;

}
.countinputbox{
    display:flex;
    justify-content: space-between;
}
.radiobutton{
    margin-top: 50px;
}
.deleteele{
    padding-top: 50px;
    color:crimson;
}
.button{
    margin-top: 50px;
    background-color: black;
    color:blanchedalmond;
    border-radius:10px;
}
</style>