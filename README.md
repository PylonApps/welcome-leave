# Pylon welcome/leave system
To use this module in [Pylon](https://pylon.bot/), go to the editor, create a new file called `welcome-leave.ts`, copy the contents of this repositorys `welcome-leave.ts` into it and then put the following in your `main.ts`:
```ts
import './welcome-leave';
```

This module requires a [pxlAPI](https://pxlapi.dev/) account for image generation. 
If you have a pxlAPI application token, expose it in your `main.ts` as follows: `global.PXLAPI_TOKEN = '<your token here>';`.  
You will also need to expose the channel you want to send the join/leave messages in like this: `global.JOIN_LEAVE_CHANNEL = '<channel id here>';`
An example `main.ts` would look like this:
```ts
global.PXLAPI_TOKEN = 'f03bc4bd35177305bc43cf3abb072436';
global.JOIN_LEAVE_CHANNEL = '730490621088759941';
import './welcome-leave';
```