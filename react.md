# react

### Components

```jsx
// "custom" HTML element
function Component(props){
    const [text, setText] = useState('')
    return <input className="text-input"
        style={{color: props.color}}
        value={text}
        onChange={e=> setText(e.target.value)}
    />
}
```

Then you can use it like this:
```jsx
// the text color of the <input /> inside the Component
// will be green
function App(){
    return <Component color="green">
}
```

### props

props can be anything at all

```jsx
// variable prop
// this is for passing data DOWN into a child component
<Component color="green">
```

```jsx
// function prop
// for passing data UP from child to parent
<Component onChange={e=> console.log(e)}>
```

### props vs state

Props act just like state in a component. If a prop changes its value, it will re-render the component, just like if state changes.

If you need to share "state" between components, then you should create your "state" variables in a common Parent component.

```jsx
function SettingsMenu(){
    const [username, setUsername] = useState('')
    return <section>
        <NamePicker setUsername={setUsername} username={username}>
        <UserProfile username={username}>
    </section>
}
```

In the above example, the NamePicker and the UserProfile dont manage the username "state"... instead, the "username" state is managed in their shared Parent (SettingsMenu) 

### state

"State" is a magical variable that React knows to "watch"... anytime a "state" variable changes, React will update your application visually to reflect that change

```jsx
function NamePicker(props){
    const [username, setUsername] = useState('')
    function saveUsername {
        props.setUsername(username)
    }
    return <main>
        <input value={username}
            onChange={e=> setUsername(e.target.value)}
        />
        <button onClick={saveUsername}>OK</button>
    </main>
}
```

