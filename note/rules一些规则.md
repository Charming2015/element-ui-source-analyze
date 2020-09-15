#### 代码基本结构

- packages

```
/packages
	/component
		index.js
		/src
			main.vue
/other-components
	...
```



- scss

```
/packages
	/theme-chalk
		/lib   ==================================    打包目录
		/src
			/common    ============================    公用文件
				popup.scss    =======================    弹窗相关样式
				transition.scss    ==================    动画样式
				var.scss    =========================    变量
			/fonts    =============================    icon字体
			/mixins
				config.scss    ======================    BEM的config
				function.scss    ====================    辅助函数
				mixins.scss    ======================    b(),e(),m()等mixin
				utils.scss    =======================    clearfix等工具
			[componentName].scss    ===============    组件样式文件
			base.scss    ==========================    引入动画和icon
			index.scss    =========================    入口文件
```





#### 基础色彩系统

```scss
/// color|1|Brand Color|0
$--color-primary: #409EFF !default;
/// color|1|Background Color|4
$--color-white: #FFFFFF !default;
/// color|1|Background Color|4
$--color-black: #000000 !default;
/// color|1|Functional Color|1
$--color-success: #67C23A !default;
/// color|1|Functional Color|1
$--color-warning: #E6A23C !default;
/// color|1|Functional Color|1
$--color-danger: #F56C6C !default;
/// color|1|Functional Color|1
$--color-info: #909399 !default;
```



#### 字体系统

```css
font-family: "Helvetica Neue",Helvetica,"PingFang SC","Hiragino Sans GB","Microsoft YaHei","微软雅黑",Arial,sans-serif;
```





#### 边框-圆角系统

```scss
/* Border
-------------------------- */
$--border-width-base: 1px !default;
$--border-style-base: solid !default;
$--border-color-hover: $--color-text-placeholder !default;
$--border-base: $--border-width-base $--border-style-base $--border-color-base !default;
/// borderRadius|1|Radius|0
$--border-radius-base: 4px !default;
/// borderRadius|1|Radius|0
$--border-radius-small: 2px !default;
/// borderRadius|1|Radius|0
$--border-radius-circle: 100% !default;
/// borderRadius|1|Radius|0
$--border-radius-zero: 0 !default;
```



#### icon图标

定义字体和content

```scss
font-family: 'element-icons'

.el-icon-ice-cream-round:before {
  content: "\e6a0";
}
```

