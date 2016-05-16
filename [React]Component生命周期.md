![引用自http://www.race604.com/react-native-component-lifecycle/](http://7rf9ir.com1.z0.glb.clouddn.com/3-3-component-lifecycle.jpg)





生命周期 | 调用次数 | 能否使用setSate()
-----|-----|-----
getDefaultProps | 1(全局调用一次) | 否
getInitialState | 1 | 	否
componentWillMount | 	1 | 是
render | >=1 | 否
componentDidMount | 1 | 是
componentWillReceiveProps | >=0 | 是
shouldComponentUpdate | >=0 | 否
componentWillUpdate | >=0 | 否
componentDidUpdate | >=0 | 是
componentWillUnmount | 1 | 否

![React生命周期](https://raw.githubusercontent.com/cuitianze/React-ReactNative-Redux_NOTEBOOK/master/asserts/images/%5BReact%5DComponent%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F/React%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F.png)
