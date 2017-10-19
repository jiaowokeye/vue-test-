    <script>
        var v = new Vue({
            el:"#div1",
            data:{//数据
                message:"welcome",
                show:true
            },
            methods:{
                alert:function(){

                }
            }
        });
    </script>

    //常用指令
    v-model   input数据绑定   <input  type="text" v-model="message" />
    循环：
    v-for =  "(value,index) in arr"  //array
    v-for="(value,key) in json"  //json 
    事件：
    v-on:click="alert()";   //挂在methods上
    v-on:click 等价于  @click
    @click="alert($event,a,b)";
    事件冒泡：
            阻止冒泡 
            a)  ev.cancelBubble = true;
            b) @click.stop="alert();";
    默认行为（默认事件）；
            a)  ev.preventDefault();
            b)  @contentmenu.prevent="";
    键盘事件；
            @keydown    $event.keyCode;
            常用键：
                    回车;
                            a) @keydown.13="";
                    上，下，左，右
            @keydown.






    this----------Vue对象   指v
    显示隐藏：
    v-show="true/false";
