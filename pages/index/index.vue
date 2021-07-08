<template>
    <Tabs
        :TabList="TabList"
        :currentTab="current"
        @tabs="tabsChange"
    >
        <TabPane>
            <view>1</view>
        </TabPane>
        <TabPane>
            <view>2</view>
        </TabPane>
        <TabPane>
            <view>3</view>
        </TabPane>
		<TabPane>
		    <view>4</view>
		</TabPane>
		<TabPane>
		    <view>5</view>
		</TabPane>
		<TabPane>
		    <view>6</view>
		</TabPane>
		<TabPane>
		    <view>7</view>
		</TabPane>
		<TabPane>
		    <view>8</view>
		</TabPane>
		<TabPane>
		    <view>9</view>
		</TabPane>
    </Tabs>
</template> 
  
<script>  
import Tabs from '@/components/tabs/tabs.vue'
import TabPane from '@/components/tabs/tabPane.vue'

export default {
    data(){
        return{
            current:0,
            TabList:[
                {title:'商品介绍'},
                {title:'规格参数'},
                {title:'售后保障'},
				{title:'售后保障'},
				{title:'售后保障'},
				{title:'售后保障'},
				{title:'售后保障'},
				{title:'售后保障'},
				{title:'售后保障'}
            ]
        }
    },
    methods:{
        tabsChange(index){
            this.current = index
        }
    },
    components:{
        Tabs,
        TabPane
    }
}
</script>

<style>
	
</style>