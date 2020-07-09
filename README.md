# Pylon welcome/leave system
To use this module in [Pylon](https://pylon.bot/), go to the editor, create a new file called `welcome-leave.ts`, copy the contents of this repositorys `welcome-leave.ts` into it and then put the following in your `main.ts`:
```ts
import './welcome-leave';
```

This module requires an [fAPI](https://fapi.dreadful.tech/) account for image generation.
Please refer to the [ImageScript documentation](https://imagescript.dreadful.tech/#getting-started) on how to create one.  
If you have an fAPI access token, expose it in your `main.ts` as follows: `global.FAPI_TOKEN = '<your token here>';`.  
You will also need to expose the channel you want to send the join/leave messages in like this: `global.JOIN_LEAVE_CHANNEL = '<channel id here>';`
An example `main.ts` would look like this:
```ts
global.FAPI_TOKEN = 'f03bc4bd35177305bc43cf3abb072436';
global.JOIN_LEAVE_CHANNEL = '730490621088759941';
import './welcome-leave';
```