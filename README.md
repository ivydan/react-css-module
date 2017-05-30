# CSS Module

一个基于react、webpack、baobab-react简单实例
使用 react+Less+baobab-react+webpack 实现易于维护性的代码构建方案。

# react 中样式处理是重要一环。

react样式简介：

设置样式时需要注意：
1.自定义组件建议支持 className prop ，以让用户使用时添加自定义样式。
2.设置行内样式时要使用对象。

基本样式设置要点：
1.设置width、height这类与大小有关的样式，大部分以像素为单位，为了提高效率， react会自动对这样的属性添加px
例如： const style = { height: 10}
    注意： 有些属性处理支持px为单位，还支持数字直接作为值，此时React并不添加px 如lineHeight

2.使用className库
    let div1Class = classNames({
        'div1':true,
        'btn-pressed': this.props.data.btnPress,
        'btn-over' : !this.props.data.btnPress
    })

CSS Module 存在的问题
1.全局污染
2.命名混乱
3.依赖管理不彻底
4.无法共享变量
5.代码压缩不彻底

CSS Module 解决方案
1.启用cssModules





运行：
npm run start

访问http://localhost:8080/webpack-dev-server/index.html



