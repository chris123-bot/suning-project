<template>
    <div class="search-template iconfont">
        <div class="header">
            <div class="header-left" @click="back">&#xe6ec;</div>
            <div class="header-middle">
                <span>&#xe607;</span>
                <input type="text" placeholder="冰柜小型家用" />
            </div>
            <div class="header-right">搜索</div>
        </div>
        <div class="useless1"></div>
        <div class="header-content">
            <div class="header-title">热门搜索</div>
            <div class="hotWord">
                <div>口罩</div>
                <div class="f60">美的狂欢不停</div>
                <div>加湿器</div>
                <div>酸奶</div>
                <div>睡衣</div>
                <div class="f60">护发素买一送一</div>
                <div class="f60">洗发水两件五折</div>
                <div>爱国者手机U盘</div>
                <div>粉底</div>
                <div class="f60">蜜饯</div>
                <div class="f60">资生堂防晒</div>
                <div>抽纸</div>
            </div>
        </div>
        <div class="useless1"></div>
        <div class="history">
            <span>历史记录</span>
            <span>&#xe615;</span>
        </div>

        <div class="header-content">
            <div class="hotWord">
                <div>李子园</div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    methods: {
        back() {
            this.$router.go(-1);
        },
    },
};
</script>

<style scoped>
.search-template {
    width: 100%;
    background: white;
}
.header {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding: 8px;
}
.header-left {
    font-size: 25px;
    font-weight: 100;
}
.header-middle {
    display: flex;
    flex-grow: 1;
    padding: 0 10px;
}
.header-middle span {
    background-color: #f2f2f2;
    padding: 0 6px;
    display: flex;
    justify-content: center;
    align-items: center;
}
.header-middle input {
    width: 100%;
    background-color: #f2f2f2;
    border: 1px solid #eee;
}
.header-right {
    font-size: 15px;
    font-weight: 100;
    display: flex;
    justify-content: center;
    align-items: center;
}
.useless1 {
    width: 100%;
    height: 2px;
    background-color: #ddd;
}
.header-title {
    font-size: 14px;
    color: #a3a2a2;
    padding: 12px 12px 8px 12px;
}
.header-content {
    width: 100%;
    padding: 0 0 14px 0;
}
.hotWord {
    width: 100%;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-between;
    padding: 0px 12px;
}
.hotWord > div {
    width: 30%;
    text-align: center;
    font-size: 14px;
    background-color: #f2f2f2;
    flex-shrink: 0;
    padding: 8px 0px;
    margin-top: 10px;
}
.f60 {
    color: #f60;
}
.history {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding: 18px 12px;
}
.history span {
    font-size: 15px;
    color: #999;
}
</style>