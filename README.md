# Website Cheat Code Script
Simple small script written in JavaScript that allows you to use cheat code or "Konami Code" on your website.

[Demo](https://geril.github.io/js-cheat-codes/demo/)

## How to use
**1. Include library to your website**

To start using this library you need to include script on your website using script tag.
```
<script src="./js-cheat-codes.min.js"></script>
```
**2. Initialize library**

After script is included on your website you need to initialize library. To make sure that everything will work fine make sure that you have included following code as the last thing in your body tag. 
```
<script>
// Simplest example
jsCheat.init({
    code: 'cheat',
    callback: () => { console.log('So cool!') },
});
</script>
```

## Documentation
Options object passed to init function allows you to use following options:

**Code (required)**
```
// Code Array
code: ['ArrowUp', 'ArrowDown', 'ArrowLeft', 'ArrowRight']
// Simple string cheat code
code: 'secret'
```

**Callback function (required)**

Function that runs after correct cheat code is entered. This function is not required only in debug mode. When using `debug: true` default success function will be fired that writes information about correct code entered in your browser's console.

**Debug option**

If you want to enable "debug" window that shows informations about user's input and current code you can use debug option.
```
debug: true
```