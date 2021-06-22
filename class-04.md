1.  What is a ‘Controlled Component’?
n HTML, form elements such as <input>, <textarea>, and <select> typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().
  
  
3.  Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
  ince the value attribute is set on our form element, the displayed value will always be this.state.value, making the React state the source of truth. Since handleChange runs on every keystroke to update the React state, the displayed value will update as the user types.
  
  
4.  How do we target what the user is entering if we have an event handler on an input field?
   handleChange(event) {
    this.setState({value: event.target.value});
  }
  
  
 1. Why would we use a ternary operator?
  Shorten your if statements into one line of code with the conditional operator

2.  Rewrite the following statement using a ternary statement
  
          if(x===y){
       console.log(true);
        } else {
       console.log(false);
        }
  
  
  to
        x === y ? 'Yes' : 'No';
