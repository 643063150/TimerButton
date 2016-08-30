# TimerButton
点击进行倒计时的按钮控件

##效果图

![img](https://github.com/SmallLee/TimerButton/blob/master/GIF.gif)

##使用
1.布局文件

```Java
 <com.fang.timerbutton.TimerButton
       android:id = "@+id/timerbutton"
       android:layout_width="wrap_content"
       android:layout_height="wrap_content"
       android:text = "发送验证码"
       android:textColor = "@drawable/tv_selector"
       android:background = "@drawable/bt_selector"
       />
```
关于Button的样式因为不同项目需求不一样，就由大家自己去实现

2.代码

```Java
 timerButton.setTimeLength(10*1000)
              .setTextBefore("点击获取验证码")//点击之前显示的文字
              .setTextAfter("秒后重新获取");//点击之后显示的文字
              //点击监听
        timerButton.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
            }
        });
```
