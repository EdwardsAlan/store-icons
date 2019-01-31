# Dreamstore Icons

## Description

All the icons that Dreamstore apps use.

## Release schedule

| Release  | Status              | Initial Release | Maintenance LTS Start | End-of-life | Dreamstore Compatibility
| :--:     | :---:               |  :---:          | :---:                 | :---:       | :---: 
| [0.x]    | **Current Release** |  2019-01-30     | -----------           | ----------  | 2.x

## Table of Contents
- [Usage](#usage)
- [Concepts](#concepts)
    - [Icons API](#icons-api)
- [Icons List](#icons-list)
    - [High Priority Actions](#high-priority-actions)
    - [Middle Priority Actions](#middle-priority-actions)
    - [Informational](#informational)
    - [Navigation](#navigation)
    - [Status Indicators](#status-indicators)
- [Testing](#testing)

## Usage

To use any icon of this project follow the steps below:

1. Add into the dependencies of your `manifest.json` and use it like a npm module.
    ```json
    "dependencies": {
        "vtex.dreamstore-icons": "0.x"
    }
    ```

2. Import and use it into your code, for example: 
    ```js
    ...
    import { IconMenu } from 'vtex.dreamstore-icons'
    ...
    const YourComponent = props => (
        ...
        <IconMenu />
        ...
    )
    ```

## Concepts

### Icons API

Any icon can receive the following props:
- **size**: Desired size (default is 16).
- **isActive**: Whenever the icon is active
- **activeClassName**: The className it should have if active
- **mutedClassName**: The className it should have if not active
- **...props**: Its is importat to notice that any other ```<svg>``` prop passed will work with any icon as well.

Some components suport modifiers. These are props that define the icon type, orientation or state.
- **type**: possible values are *solid*, *line*, *outline*
- **orientation**: possible values are *up*, *down*, *left*, *right*
- **state**: possible values are *on*, *off*

## Icons List

### High Priority Actions
| Component | Types | Orientation | State 
| :---:     |:---:  | :---:       | :---:      
| [IconArrowBack](https://github.com/vtex-apps/dreamstore-icons/blob/feature/docs/react/IconArrowBack.js) | 🚫 | 🚫 | 🚫 
| [IconAssistantSales](https://github.com/vtex-apps/dreamstore-icons/blob/feature/docs/react/IconAssistantSales.js) | 🚫 | 🚫 | 🚫  
| [IconProfile](https://github.com/vtex-apps/dreamstore-icons/blob/feature/docs/react/IconProfile.js) | 🚫 | 🚫 | 🚫 
| [IconCart](https://github.com/vtex-apps/dreamstore-icons/blob/feature/docs/react/IconCart.js) | 🚫 | 🚫 | 🚫 
| [IconSearch](https://github.com/vtex-apps/dreamstore-icons/blob/feature/docs/react/IconSearch.js) | 🚫 | 🚫 | 🚫 
| [IconDelete](https://github.com/vtex-apps/dreamstore-icons/blob/feature/docs/react/IconDelete.js) | 🚫 | 🚫 | 🚫 
| [IconMenu](https://github.com/vtex-apps/dreamstore-icons/blob/feature/docs/react/IconMenu.js) | 🚫 | 🚫 | 🚫 

### Middle Priority Actions
| Component | Types | Orientation | State 
| :---:     |:---:  | :---:       | :---:      
| [IconEyesight]() | solid \| outline |  🚫 | on \| off 
| [IconMinus]() | solid \| outline \| line | 🚫 | 🚫
| [IconPlus]() | solid \| outline \| line | 🚫 | 🚫
| [IconSingleItem]() | 🚫 | 🚫 | 🚫 
| [IconList]() | 🚫 | 🚫 | 🚫 
| [IconGallery]() | 🚫 | 🚫 | 🚫 

### Informational
| Component | Types | Orientation | State 
| :---:     |:---:  | :---:       | :---:      
|           |       |             |

#### Navigation
| Component | Types | Orientation | State 
| :---:     |:---:  | :---:       | :---:      
| [IconCaret]() | 🚫 | up \| down \| left \| right | 🚫

### Status Indicators
| Component | Types | Orientation | State 
| :---:     |:---:  | :---:       | :---:      
| [IconClose]() | solid \| outline | 🚫 | 🚫

## Testing

To test your code you should run on your workspace:

```sh
vtex link
```
