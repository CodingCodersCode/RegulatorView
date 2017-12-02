# RegulatorView

![image](https://github.com/mochixuan/RegulatorView/blob/master/RegulatorMaster/img/main.jpg)
![image](https://github.com/mochixuan/RegulatorView/blob/master/RegulatorMaster/img/slide.gif)
![image](https://github.com/mochixuan/RegulatorView/blob/master/RegulatorMaster/img/sweep.gif)

## 1. ��Ҫ����
>- ����ƽ���
>- ����Ƶ�ɫ
>- ���ƻ�����ɫ
>- ���ƻ��εĶ���
>- ƽ��ʵ�ֵ���
>- �������Բ���������΢��

## 2. ��;
>- �յ�ң����
>- ���ֵ�λ������
>- ��ˮ��������

## 3. ʹ��

> ��Ҫ����һ��Բ������Ҿ�֪��ʲô��˼�˴����Ŀ�ʼһ������Բ�ֱ��� ��һ��Բ ʵ��Բ:firstCircle �ڶ���Բ��: secondCircle ������Բ:���β�ɫԲ��: threeCircle

#####  attrs
```
      <attr name="three_circle_radius" format="dimension"/>
        
        <attr name="first_circle_color" format="color"/>
        <attr name="second_circle_color" format="color"/>
        <attr name="secondcircle_shadow_color" format="color"/>
        <attr name="three_circle_color" format="color"/>
        
        <attr name="second_circle_width" format="dimension"/>
        <attr name="secondcircle_shadow_width" format="dimension"/>
        <attr name="three_circle_width" format="dimension"/>
        <attr name="gap1_width" format="dimension"/>
        
        <attr name="three_ring_angle" format="integer"/>
        <attr name="second_scale" format="float"/>
        
        <attr name="pointer_color" format="color"/>
        <attr name="pointer_scale" format="float"/>
        <attr name="pointer_width" format="dimension"/>

        <attr name="symbol" format="string"/>
        <attr name="center_title" format="string"/>
        <attr name="bottom_title" format="string"/>

        <attr name="symbol_color" format="color"/>
        <attr name="center_title_color" format="color"/>
        <attr name="bottom_title_color" format="color"/>

        <attr name="symbol_size" format="dimension"/>
        <attr name="center_title_size" format="dimension"/>
        <attr name="bottom_title_size" format="dimension"/>

        <attr name="bottomcenter_gap" format="dimension"/>
        <attr name="symbolcenter_gap" format="dimension"/>
        <attr name="symbolmovetop_gap" format="dimension"/>

        <attr name="backlight_durtion" format="integer"/>
        <attr name="isopen_backlightanim" format="boolean"/>
        <attr name="is_forbid_slide" format="boolean"/>
```

##### xml 
```
<!--���������Լ������־�֪��������ʵ��΢��ÿһ������-->
<com.wx.regulatorview.RegulatorView
    android:id="@+id/regulator_view"
    android:layout_width="match_parent"
    android:layout_height="360dp"
    app:symbol="��"
    app:center_title="10"
    app:bottom_title="Auto" />
```

##### java

```
mRegulatorView = findViewById(R.id.regulator_view);
 mColors = new int[]{0xff2ab62d,0xff2ab62d, 0xff56f318, 0xff8ff318, 0xffd2f318, 0xfff3b318, 0xfff36a18, 0xffe73046, 0xffff0000,0xffff0000};
mRegulatorView.setThreeCircleColors(mColors);
mRegulatorView.setProgressChangeListener(new OnProgressChangeListener() {
     @Override
     public void onProgress(float progress) {
                
     }
});
```

## 4.����

����û�н������ϴ���jcenter���������Ŀ��Ҫ����Ӧ��ҲҪС��Χ�޸ģ����Ҵ�����ʵ��һ�������࣬��Ŀ����ֱ��ճ�������ʡ�


