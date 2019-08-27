## 大转盘

点击抽奖，转盘转动，结束后弹出对应奖项

## 注意

因为抽奖涉及到奖品, 应该是后端控制中奖奖项，前端只用于展示

## 引入

```json
{
  "usingComponents": {
    "s-wheel": "/components/s-wheel/index"
  }
}
```

## 使用

```html
<s-wheel award-numer="{{award}}" disabled="{{disabled}}" bind:success="wheelSuccess"></s-wheel>
```

## API

| 参数         | 类型     | 描述                           | 默认值 |
| ------------ | -------- | ------------------------------ | ------ |
| areaNumber   | Number   | 奖项个数                       | 6      |
| awardNumer   | Number   | 中奖区域 从 1 开始             | 1      |
| speed        | Number   | 旋转速度                       | 16     |
| mode         | Number   | 抽奖模式 1:转盘旋转 2:指针旋转 | 1      |
| bind:success | Function | 成功后的回调函数               | -      |

## 效果展示

![logo](../_images/1.gif)