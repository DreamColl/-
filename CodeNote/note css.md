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

3. **Selectors Level 3**

   ```css
   子串匹配的属性选择器， E[attribute^="value"]， E[attribute$="value"]， E[attribute*="value"]

   新的伪类：:target， :enabled 和 :disabled， :checked， :indeterminate， :root， :nth-child 和 :nth-last-child， :nth-of-type 和 :nth-last-of-type， :last-child， :first-of-type 和 :last-of-type， :only-child 和 :only-of-type， :empty， 和 :not。

   伪元素使用两个冒号而不是一个来表示：:after 变为 ::after， :before 变为 ::before， :first-letter 变为 ::first-letter， 还有 :first-line 变为 ::first-line。

   新的 general sibling combinator(普通兄弟选择器)  ( h1~pre )。
   ```

   ​

4. ​