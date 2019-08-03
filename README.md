# React cheatsheet

React is a unidiractional library

https://github.com/enaqx/awesome-react

API Reference   | Description  
---             | ---   
**Component**                       | lets you split the UI into independent, reusable pieces in isolation
**State**                           | Can manage the dynamic data in a component
**Properties**                      | Can access the proprties passed to components
**Fragment**                        | Can be used to return multiple nested children without wrapping dom/node name
**Children**                        | {this.props.children} to access the children from the usage
**defaultProps**                    | Can be defined on the class, to set the default values. It is used only in the undefined props
**Initial State**                   | Can be set in the constructor
**Functional Component**            | State less component, which gets the properties as first parameter
**Pure Component**                  | Doesn’t rerender if props/state hasn’t changed; done via shallow comparison.
**Component APIs**                  | [Hit me](https://reactjs.org/docs/react-component.html) 
**LC - constructor (props)**        | Before rendering
**LC - componentWillMount()**       | Don’t use this
**LC - render()**                   | Render
**LC - componentDidMount()**	      | After rendering (DOM available) 
**Lc - componentWillUnmount()**	    | Before DOM removal 
**LC - componentDidCatch()**	      | Catch errors (16+)
**LC - componentDidUpdate()**       |	Do setState(), DOM operation or network calls here
**LC - shouldComponentUpdate()**    |	Skips render() if returns false
**LC - componentWillReceiveProps()**| invoked every time component recieves new props.
**LC - componentWillUpdate()**      | invoked immediately before update (new props or state)
**forceUpdate()**                   | forces a re-render; AVOID if possible
**Dom node access**                 | `<input ref={el => this.input = el} />, componentDidMount () { this.input.focus() }`
**Dom event**                       | `<input onChange={event => this.onChange(event)} />, onChange (event) { }`
**Transfer properties**             | `<Children {...this.props} />`
**Style 1**                         | `const style = { height: 10 }, <div style={style}></div>`
**Style 2**                         | `<div style={{ margin: 0, padding: 0 }}></div>`
**inner HTML**                      | `<div dangerouslySetInnerHTML={{__html: markdownify()}} />`
**Conditions**                      | `<Fragment> { showMyComponent ? <MyComponent /> : <OtherComponent /> } </Fragment>`
**Short-circuit evaluation**        | `<Fragment> { showPopup && <Popup />} </Fragment>`
**Lists**                           | `<ul> { items.map(item => <Child {...item} />) } </ul>`
**Returning multiple elements**     | `render () { return [ <li key="A">First item</li>, <li key="B">Second item</li> ] } // Keys mandatory` 
**Returning strings**               | `render() { return 'Look ma, no spans!'; }`
**Validation**                      | `PropTypes - MyComponent.propTypes = { email: PropTypes.string }`
**Custom validation**               | `MyCo.propTypes = { customProp: (props, key, componentName) => { return new Error('Validation failed!') } }`
**Contect**                         | Context provides a way to pass data through the component tree without having to pass props down manually at every level




