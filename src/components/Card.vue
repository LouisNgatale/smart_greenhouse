<template>
    <div class="widget mx-auto" 
        :class="{
            temperature: theme === 'temperature',
            humidity: theme === 'humidity',
            moisture: theme === 'moisture',
            ph: theme === 'ph',
            water_level: theme === 'water_level',
        }">
        <div class="p-2">
            <span class="banner">Temperature</span>
        </div>
        <div class="mx-2 my-3 icon">
            <img src="@/assets/icons/temperature.svg" alt="">
        </div>
        <div class="my-2 container-fluid ">
            <div class="row">
                <div class="col warehouse">
                    <p class="sub-title">Warehouse</p>
                    <p class="value">25&#176;C</p>
                </div>
                <div class="col outside">
                    <p class="sub-title">Outside</p>
                    <p class="value">25&#176;C</p>
                </div>
            </div>
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
    height: 250px;
    width: 240px;
    border-radius: 19px;
    transition: all .4s;
    transition: background-color 0.5s ease;
    padding: 10px 10px;

    

    .icon{
        display: flex;
        justify-content: center;
        align-content: center;
    }

    .icon img{
        margin: auto;
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

.widget.temperature{
    height: 250px;
    width: 240px;
    border-radius: 19px;
    border: 1px $orange solid;
    background-color: rgb(6,6,9);
    background-color: linear-gradient(39deg, rgba(6,6,9,1) 0%, rgba(14,18,36,1) 100%);
    transition: all .4s;
    transition: background-color 0.5s ease;
    padding: 10px 10px;
    &:hover{
        cursor: pointer;
        background: rgb(8,8,9);
        background-color: linear-gradient(39deg, rgba(8,8,9,1) 0%, rgba(15,12,10,1) 100%);
        box-shadow: 0px 4px 40px rgba($color: #BC7F16, $alpha: .3);
        transition: all .4s;
    }
    .banner{
        border: 1px $orange solid;
        border-radius: 5px;
        padding: 5px 8px;
        font-size: 12px;
        background: #0C0F1C;
    }
}
.widget.humidity{
    height: 250px;
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
}
.widget.moisture{
    height: 250px;
    width: 240px;
    border-radius: 19px;
    border: 1px $brown solid;
    background-color: rgb(6,6,9);
    background-color: linear-gradient(39deg, rgba(6,6,9,1) 0%, rgba(14,18,36,1) 100%);
    transition: all .4s;
    transition: background-color 0.5s ease;
    padding: 10px 10px;
    &:hover{
        cursor: pointer;
        background: rgb(8,8,9);
        background: linear-gradient(39deg, rgba(8,8,9,1) 0%, rgba(36,27,21,1) 100%);
        box-shadow: 0px 4px 40px rgba($color: #C87A49, $alpha: .3);
        transition: all .4s;
    }
    .banner{
        border: 1px $brown solid;
        border-radius: 5px;
        padding: 5px 8px;
        font-size: 12px;
        background: #0C0F1C;
    }
}
.widget.ph{
    height: 250px;
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
}
.widget.water_level{
    height: 250px;
    width: 240px;
    border-radius: 19px;
    border: 1px $purple solid;
    background-color: rgb(6,6,9);
    background-color: linear-gradient(39deg, rgba(6,6,9,1) 0%, rgba(14,18,36,1) 100%);
    transition: all .4s;
    transition: background-color 0.5s ease;
    padding: 10px 10px;
    &:hover{
        cursor: pointer;
        background: rgb(6,6,9);
        background: linear-gradient(39deg, rgba(6,6,9,1) 0%, rgba(14,18,36,1) 100%);
        box-shadow: 0px 4px 40px rgba($color: #5D46EE, $alpha: .3);
        transition: all .4s;
    }
    .banner{
        border: 1px $purple solid;
        border-radius: 5px;
        padding: 5px 8px;
        font-size: 12px;
        background: #0C0F1C;
    }
}
</style>