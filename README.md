# KeyCODE
A developer tool for `e.keyCode` in webpages. Use this app to find out the `e.keyCode` or `e.which` value to use in your JavaScript code for keyboard events like `onkeydown`, `onkeyup`, and `onkeypress`.

## How to use
Open up [http://cameronsamuels.com/keycode](http://cameronsamuels.com/keycode) and type any key to get the key code value.

In your JavaScript code you can use the following for basic usage:

```javascript
document.onkeyup = function(e) { //create a listener function for when a key is lifted up
  switch (e.keyCode || e.which) { //switch statement for evaluating the keyCode
    case 8 /* backspace */: alert('backspace'); break; //show backspace if back key was pressed
    case 13 /* enter */: alert('enter'); break; //show enter if enter key was pressed
    case 32 /* spacebar */: alert('spacebar'); break; //show spacebar if spacebar key was pressed
    default /* none of the above */: alert('other key'); break; //show other key if none of the above
  }
  alert('Ctrl Key: ' + e.ctrlKey); //show if the ctrl key was pressed. Also other modifiers can be e.altKey; e.shiftKey; e.metaKey;
}
```
## Apps
I offer a [Chrome app](https://goo.gl/eQfc6p) currently for easily checking keycodes without having to search or open a new tab. Soon I will release an Android and iOS app. Other platforms may come, including a Firefox and Opera extension, and possibly a Windows app.

## Contributing
If you want to contribute, you may fork this repo.

Also you can add issues in the issues tab if there is an uknown key or something. I will really appreciate it.

## About
Made by [Cameron Samuels](http://cameronsamuels.com) and started in June 2017 using JavaScript, HTML, and CSS.
