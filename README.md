布局文件：
<net.rippletec.layout.WaveView
android:id="@+id/wv_bg"
android:layout_width="match_parent"
android:layout_height="match_parent" />


配置代码：
//获取控件
wave_bg = (WaveView) findViewById(R.id.wv_bg);
//设置控件宽度
wave_bg.setWidth(windowWidth);
//设置控件高度
wave_bg.setHeight(tmpHeight);
//设置波浪移动方向（左右）
wave_bg.setWavingWay(WaveView.MOVE_FROM_RIGHT_TO_LEFT);
//设置波浪高度,相对于屏幕高度来说(0~1f)
wave_bg.setWaveHeight(0.8f);
//设置波长(波浪宽度百分比，相对于屏幕宽度而言)
wave_bg.setWaveWidth(1.7f);
//设置波动的速度
wave_bg.setWaveSpeed(45);
//设置波峰波谷(波峰波谷百分比，相对于波长而言)
wave_bg.setWaveCrest(0.1f);
//设置波浪颜色
wave_bg.setColor(getResources().getColor(R.color.clr_white));
//设置透明度
wave_bg.setAlpha(0.3f);
//设置水平面浮动的方向（上下）
wave_bg.setFloatingWay(WaveView.FLOAT_DOWN);
//设置最大的水平面高度
wave_bg.setMaxWaveHeight(0.8f);
//设置最低的水平面高度
wave_bg.setMinWaveHeight(0.1f);
//开始波动（水平移动）
wave_bg.startWaving();
//开始浮动（上下移动）
wave_bg.startFloating();
 
//还有一些设置方法，请直接查看源代码。
