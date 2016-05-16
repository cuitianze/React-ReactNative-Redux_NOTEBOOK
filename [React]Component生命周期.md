![]()



生命周期 | 	调用次数 | 	能否使用 |  setSate()
-----|-----
getDefaultProps | 	1(全局调用一次) | 	否
getInitialState | 	1 | 	否
componentWillMount | 	1 | 	是
render | 	>=1 | 	否
componentDidMount | 	1 | 	是
componentWillReceiveProps | 	>=0 | 	是
shouldComponentUpdate | 	>=0 | 	否
componentWillUpdate | 	>=0 | 	否
componentDidUpdate | 	>=0 | 	否
componentWillUnmount | 	1 | 	否
