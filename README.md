# rage-progressbar

Very simple Progress Bar to delay event execution.

----

# How to use

Put the `progress` folder inside `client_packages` into your `client_packages` folder (or wherever you have your client files).

Import the `progress/index.js` in your main `index.js` like it is done in my main `index.js`

You can then create a Progress Bar on the server-side with the following code:

```js
player.call('progress:start', [SECONDS, TASK, DIRECTION, EVENT, PARAMS]);
```
- **SECONDS** 
    - How many seconds is the Progress Bar running
- **TASK**
    - String which is displayed inside the progress bar
- **DIRECTION**
    - Is the event which is called after the bar has finished a server-side or client-side event
- **EVENT**
    - The event to be called afterwards
- **PARMS**
    - Additional params to send to the following event


That's pretty much it. Customize it as you want, this is as basic as possible.

`packages/Progress/index.js` contains an example with an example `/progress` command and a follow-up event.