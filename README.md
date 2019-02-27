# drop-down-input

> iview下拉搜索框扩展：可输入可下拉可搜索

> 组件入参说明：
- dropDownList: 下拉列表(Array)  **必传**
- is_show_arrow: 是否显示下拉箭头(Boolean)
- placeholder: 输入框提醒文字(String)
- maxlength: 输入框最多限制输入字符(Number, default:50)
- disabled: 输入框是否禁用(Boolean)
- value: v-model值  **必传**
- keyName: dropDownList遍历子元素keyname(String, default:label)  **必传**
- errorMsg: 错误提示(String, default:请选择或者输入正确值)

> 组件方法提供：
- onQueryChange: 搜索词改变的时候触发(query)
- focus: 输入框聚焦触发
- clear: 清空输入框的时候触发

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build
```

For detailed explanation on how things work, consult the [docs for vue-loader](http://vuejs.github.io/vue-loader).
