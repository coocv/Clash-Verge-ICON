# Clash-Verge-ICON
Clash Verge 客户端图标更换
这里我换成开发者同款
![image](https://github.com/user-attachments/assets/896eb589-084c-472c-80ca-bfab099483ca)


## 1.通过开发者工具找到代码段并调试成喜欢的样子(普通用户直接跳过）
![image](https://github.com/user-attachments/assets/8c53de9f-6516-4f69-b2f6-4bb6449baa4b)
![image](https://github.com/user-attachments/assets/1ccb67bd-427c-4844-b7e4-d7831c712997)

## 2.设置>主题设置
![image](https://github.com/user-attachments/assets/1b7e0245-8892-467b-9e23-8a79006ce8ba)

## 2.点击编辑CSS
![image](https://github.com/user-attachments/assets/f9b006af-cac4-4942-a5ef-668ccfc9a56a)

## 3.粘贴CSS代码并保存

```
/* 隐藏第一个SVG */
.the-logo>div svg:first-of-type {
  display: none;
}

/* 在 .the-logo > div 中创建一个新的 div */
.the-logo>div::before {
  content: '';
  display: block;
  width: 46px;
  /* 设置与第一个SVG一样的宽度 */
  height: 46px;
  /* 设置与第一个SVG一样的高度 */
  left: 5px;
  bottom: 8px;
  background-image: url('https://clashverge.net/wp-content/uploads/2023/11/cropped-logo.png');
   /* 把链接更换为自定义图片 */
  background-size: contain;
  /* 保持比例 */
  background-repeat: no-repeat;
  background-position: center;
  position: absolute;
  /* 确保它可以精确定位 */
}

/* 保证第二个SVG正常显示，不受影响 */
.the-logo>div svg:nth-of-type(2) {
  display: block;
  margin-left: 40px;
}
```

## 4.查看效果
![image](https://github.com/user-attachments/assets/31681c67-3fb1-4507-b12b-45bf24348989)


