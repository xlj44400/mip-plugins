# mip-ck-ad
### 康网的问答详情页面的直投广告组件

| 描述 | 展示页面直投广告|
|---|---|
|可用性	|完成 |
|所需脚本| mip-ck-ad.js |

# 使用方法

在MIP HTML中,直接使用标签, 用于正常显示直投的广告。示例如下:
```
 <mip-ck-ad></mip-ck-ad>
```


# 属性
组件涉及的属性字段:康网广告位id(ck-ad-pid)、康网广告位关键词(ck-ad-keywords)、懒加载(lazy)。

+ 康网广告位id(ck-ad-pid)
    - 是否必填: 是
    - 说明: 指定康网直投广告位唯一ID
    
+ 康网广告分类id(ck-ad-cateid)
    - 是否必填: 否
    - 说明: 康网直投广告关键词组,多词用,分隔例:`ck-ad-cateid="瘦身,性病,减肥"`, 如果没有指定则直接获取`#tags`的`data-cateid`
    
+ 懒加载(lazy) (true | false)
    - 是否必填: 否
    - 说明: 加载广告的方式,默认是true,执行懒加载,如果设置false,则表示加载渲染页面时,直接加载对应的直投广告