# sm-city-picker
### 基于MSUI开发的省市二级滚轮联动插件

> 效果图  
![screen-capture](https://github.com/jacobcyl/sm-city-picker/blob/master/screen-capture.gif)

### 用法
```html
<link rel="stylesheet" href="//g.alicdn.com/msui/sm/0.6.2/css/sm.min.css">
<script type='text/javascript' src='//g.alicdn.com/sj/lib/zepto/zepto.min.js' charset='utf-8'></script>
<script type='text/javascript' src='//g.alicdn.com/msui/sm/0.6.2/js/sm.min.js' charset='utf-8'></script>
<script type="text/javascript" src="sm-city-picker.js" charset="utf-8"></script>
<li>
    <div class="item-content">
        <div class="item-media"><i class="icon icon-form-name"></i></div>
        <div class="item-inner">
            <div class="item-title label">地点</div>
            <div class="item-input">
                <input type="text" required name="place_name" placeholder="请选择所在地区" id="city-picker">
                <input type="hidden" id="province" name="province">
                <input type="hidden" id="place" name="place">
            </div>
        </div>
    </div>
</li>
```

```javascript
$("#city-picker").cityPicker({
            toolbarTemplate: '<header class="bar bar-nav">\
            <button class="button button-link pull-right close-picker">确定</button>\
            <h1 class="title">选择所在地址</h1>\
            </header>',
            province: '#province',//省输入框,一般都是隐藏的，获取身份ID
            place: '#place' //城市输入框，一般都是隐藏的，获取城市ID
        });
```
