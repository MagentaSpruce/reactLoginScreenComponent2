# reactLoginScreenComponent2
Created with React

This simple login component presents a register or a login form for users. It can easily be styled and cross-utilized. 

Building this React app has helped me to better learn and practice:

A brief overview of the pertinent React code is given below.

Create the login form using conditions.
```React
function Form(props) {
  return (
    <form className="form">
      <input type="text" placeholder="Username" />
      <input type="password" placeholder="Password" />
      {!props.isRegistered && (
        <input type="password" placeholder="Confirm Password" />
      )}

      <button type="submit">{props.isRegistered ? "Login" : "Register"}</button>
    </form>
  );
}
```

Determine the conditions.
```React
var userIsRegistered = false;

function App() {
  return (
    <div className="container">
      <Form isRegistered={userIsRegistered} />
    </div>
  );
}
```

Render.
```React
ReactDOM.render(<App />, document.getElementById("root"));
```

***End Walkthrough
