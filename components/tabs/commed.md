* 使用stylus预处理器，可能需要自己添加一下
 * 引入tabs 和tabPane组件  
    为tabs 传入 
    tablist（tab标题），
    currentTab（选中的tab）， 
    @tabs事件  改变选中的tabs
    TabList:[
        {title:'商品介绍'},
        {title:'规格参数'},
        {title:'售后保障'}
    ]  
    TabPane 根据 tab的多少添加。  
    更新：  
        在tabPane区域添加了滑动手指事件。横向滑动切换tab。  
        在tabs.vue中的  tabChange方法中发布了全局事件，不需要可以注释掉。这里主要方便tabpane中的内容监听 tabs的切换做出响应。  