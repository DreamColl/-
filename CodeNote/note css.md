# CSS记录

1. 1px线

   ```css
   // 上下两条 颜色偏蓝
   box-shadow: 0 1px 1px -1px rgba(0, 0, 0, 0.5);

   // 按需添加
   li{
   	position: relative;
   	border:none;
   }
   li:after{
       content: '';
   	position: absolute;
   	left: 0;
   	background: #000;
   	width: 100%;
   	height: 1px;
   	transform: scaleY(0.5);
   	transform-origin: 0 0;
   }

   ```

   ​

2. 四个半椭圆

   ```css
   向上半椭圆
   brouder-radius: 50%/100% 100% 0 0

   向下半椭圆
   brouder-radius: 50%/0 0 100% 100%

   向左半椭圆
   brouder-radius: 100% 0 0 100%/50%

   向右半椭圆
   brouder-radius: 0 100% 100% 0/50%
   ```

   ​

3. ​