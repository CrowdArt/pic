## Callback functions:
* onClick - we can wire up onClick handler to a div
* onChange
* onSubmit


Two ways of creating the same function:
```javascript
    onFormSubmit(event) {
        event.preventDefault();
    }

    onFormSubmit = (event) => {
        event.preventDefault();

        console.log(this.state.term);
    }
```
```jsx
<form onSubmit = {event => this.onFormSubmit(event)} className = "ui form">
```

Communicating between components using prop system.  Prop system allows us to pass information from parent component down to a child.