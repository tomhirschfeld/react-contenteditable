react-contenteditable
=====================

React component for a div with editable contents
This fork is to make minor changes to get this component to play nice with webpack


## Usage
```javascript
  var ContentEditable = require("react-contenteditable");
  var MyComponent = React.createClass({
    getInitialState: function(){
      return {html: "<b>Hello <i>World</i></b>"};
    },

    handleChange: function(evt){
      this.setState({html: evt.target.value});
    },

    render: function(){
      return <ContentEditable html={this.state.html} onChange={this.handleChange}/>
    }
  });
```
