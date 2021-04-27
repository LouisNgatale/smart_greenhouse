<template>
    <div class="widget mx-auto px-3" >
        <div class="py-2">
            <span >Ventilation</span>
        </div>
        <div class="icon">
            <img src="@/assets/icons/water.svg" alt="">
            <input type="checkbox" value="ventilate" name="" id="ventilation">
        </div>
    
    </div>
</template>

<script>
export default {
    props:[
        'theme'
    ]
    
}
</script>

<style lang="scss" scoped>
.container-fluid{
    padding: 0 5px;
}
p{
    margin: 0;
}
.widget{
    height: 104px;
    width: 240px;
    border-radius: 19px;
    border: 1px $cyan solid;
    background-color: rgb(6,6,9);
    background-color: linear-gradient(39deg, rgba(6,6,9,1) 0%, rgba(14,18,36,1) 100%);
    transition: all .4s;
    transition: background-color 0.5s ease;
    padding: 10px 10px;
    &:hover{
        cursor: pointer;
        background: rgb(6,6,9);
        background: linear-gradient(39deg, rgba(6,6,9,1) 0%, rgba(14,18,36,1) 100%);
        box-shadow: 0px 4px 40px rgba($color: #36BBA8, $alpha: .3);
        transition: all .4s;
    }
    .banner{
        border: 1px $cyan solid;
        border-radius: 5px;
        padding: 5px 8px;
        font-size: 12px;
        background: #0C0F1C;
    }
    

   .icon{
        display: flex; 
        justify-content: space-between;
        align-items: center;
        input[type="checkbox"]{
            position: relative;
            width: 40px;
            height: 20px;
            border: 2px solid #c6c6c6;
            -webkit-appearance: none;
            outline: none;
            border-radius: 20px;
            box-shadow: inset 0 0 5px rgba(0,0,0,.2);
            transition:all .5s;
        }
        input:checked[type="checkbox"]{
            border: 2px solid $cyan;
            background: rgb(6,107,125);
            background: linear-gradient(329deg, rgba(6,107,125,1) 0%, rgba(12,213,249,1) 100%);
        }
        input[type="checkbox"]:before{
            content: '';
            position: absolute;
            width: 18px;
            height: 18px;
            border-radius: 10px;
            top: -1px;
            left: 0px;
            transform: scale(1.1);
            background: #c6c6c6;
            transition: all .5s;
        }
        input:checked[type="checkbox"]:before{
            left: 20px;
            background: #0B0F1A;
            transition: all .5s;
        }
        
    }

    .icon img{
        display: inline-block;
    }
    .sub-title{
        color: $grey;
        font-size: 15px;
    }
    .value{
        color: $grey;
        font-size: 30px;
        font-weight: bold;
    }
    .outside{
        text-align: left;
    }
    .warehouse{
        text-align: right;
    }
}

</style>