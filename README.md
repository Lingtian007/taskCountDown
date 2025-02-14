# 基于Js单例模式实现仿支付宝活动 倒计时任务悬浮球
## taskCountDown

```js
// 引入
<script src='./allDayArticleFtl/js/taskCountDown.js'></script>;
// 初始化
// 初始化单例
const container = document.body;
// 创建倒计时实例，设置倒计时参数和回调函数
const countdown = new Countdown(
  {
    // 倒计时总秒数
    seconds: 30,
    // 倒计时结束时的回调函数
    finish: () => {
      // 打印倒计时结束的日志
      console.log(`%c ==当前  任务完成了==>`, "background: green; color: white");
    },
    // 倒计时显示框的位置
    top: "",
    bottom: "180px",
    left: "",
    right: "30px",
  },
  // 倒计时显示的容器
  container
);

// 启动倒计时
countdown.start();

// 如果需要重置倒计时，可以调用：
// countdown.reset();
// countdown.start();
```
