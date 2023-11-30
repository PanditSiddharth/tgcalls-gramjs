# Gram TGCalls [![Mentioned in Awesome Telegram Calls](https://awesome.re/mentioned-badge-flat.svg)](https://github.com/tgcalls/awesome-tgcalls)

An operative library for Telegram calls and a tgcallsjs helper.

## Features

-   Super light & easy-to-use.
-   Smart stream function.
-   Native controls: pause, resume, mute, unmute.
-   Call helpers: join, edit, leave.

## Installation

```shell
npm i tgcalls-gramjs
```

## Example usage with audio

```js
const { GramTGCalls, gramjs } = require("tgcalls-gramjs");

// Replace these values with actual values
const apiId = 123456;
const apiHash = "392ykiyourhashhere";
const stringSession = "";

(async () => {
 const client = await gramjs(apiId, apiHash, stringSession);
  console.log(client.session.save()); // use this value in stringSession after 1 time generate
  let tg = new GramTGCalls(client, "groupusername");
  tg.streamAudio("./audio.mp3");
})();

```

## Docs

The docs can be found [here](https://tgcallsjs.github.io/gram-tgcalls).  

## Credits

-   Structure inspired from Telethon bridge in [MarshalX/tgcalls](https://github.com/MarshalX/tgcalls).  
-   Video support by [@Laky-64](https://github.com/Laky-64).  
-   Latest version with easiness by @PanditSiddharth  

inherited: tgcalls -> gram-tgcalls -> tgcalls-gramjs  

