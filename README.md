# react-native-scrolltable
基于React Native封装的频道切换组件

## Installation

```bash
npm install react-native-scrolltable --save
```
```bash
yarn add react-native-scrolltable --save
```

## Import into your project
```js
import ScrollTable from "react-native-scrolltable";
```

## Examle useage

```js
<ScrollTable 
    //initialIndex={0}
    labels={[
      { key: 0, title: "精选" },
      { key: 1, title: "推荐" },
      { key: 2, title: "热门" },
    ]}
    labelStyle={{ color: "#FFFFFF", fontSize: 14 }}
    tintColor="blue"
    //style={{ width: 200, height: 40 }}
    onChange={e => console.log(e)}
/>
```

## Properties
属性  | 描述    | 类型  | 默认    
------ | ------ | ------  | ------
initialIndex  | 初始Index | ```PropTypes.number ``` | ``` 0 ```
labels  | 频道数组 | ```PropTypes.array ``` | ``` [{ key: 0, title: "精选" }, { key: 2, title: "热门" }] ```
labelStyle | 频道标题样式  | ``` PropTypes.object ``` | ``` { color: "#FFFFFF", fontSize: 14 } ```  
tintColor | 活跃状态标题颜色  | ``` PropTypes.string ```  | "#12cdb0"' 
onChange | 频道切换回调  | ``` PropTypes.func ```  |
style | 组件样式  | ``` PropTypes.object ```  |
