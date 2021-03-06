# Checkbox

The Checkbox is part of the *tobit-chayns_components* package. It can be installed via npm:

    npm install -S tobit-chayns_components@latest


## Usage of the Checkbox
The checkbox has to be imported:

```jsx
import {Checkbox} from 'tobit-chayns_components/react-chayns-checkbox';
```


You can use the checkbox like this:
```jsx
<Checkbox onChange={ (value) => { console.log(value); }} />
```

## Props
The following properties can be set on the Checkbox-Component

| Property            | Description                                                                                         | Type          | Default Value |
|---------------------|-----------------------------------------------------------------------------------------------------|---------------|---------------|
| style               | Additional styles that should be set to the checkbox                                                | Object        |               |
| className           | Additional CSS-Classes that should be add to the checkbox                                           | String        |               |
| label               | Label that will be shown next to the checkbox                                                       | String        |               |
| dangerouslySetLabel | Label that will be shown next to the checkbox (not ToggleButton)                                    | String (HTML) |               |
| children            | Label that will be shown next to the checkbox                                                       | String        |               |
| onChange            | onChange-event. Returns true or false                                                               | function      |               |
| toggleButton        | Renders checkbox as toggleButton (see [chayns-css wiki](https://github.com/TobitSoftware/chayns-css/wiki/form-elements#toggle-button)) | bool | false  |
| checked             | Set the default value of the checkbox                                                               | bool          | *deprecated*  |
| defaultChecked      | Set the default value of the checkbox                                                               | bool          | false         |
| staticChecked       | Set the value of the checkbox (like normal checked prop)                                            | bool          | false         |
| disabled            | Disables the checkbox                                                                               | bool          | false         |
| tooltip             | Tooltip that will be shown behind the label                                                         | String        |               |



### Examples
#### ToggleButton
```jsx
<Checkbox
    label="This is a toggle button"
    toggleButton={true}
    onChange={ (value) => { console.log(value); }}
/>
```
#### Checkbox
```jsx
<Checkbox
    onChange={ (value) => { console.log(value); }}
    disabled={true}
>
    This is a normal checkbox
</Checkbox>
```
