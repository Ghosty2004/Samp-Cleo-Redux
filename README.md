# Cleo Redux for SA:MP client

`Warning:` I'm not done with every natives, but I will try to add all

# Installation:
1. Download `Cleo-Redux` from https://github.com/cleolibrary/CLEO-Redux/releases/
2. Replace `sa.json` from `/cleo/.config/` with <a href="https://github.com/Ghosty2004/Samp-Cleo-Redux/blob/master/.config/sa.json">this</a>

Example of usage with JS:
```js
/// <reference path=".config/sa.d.ts" />

import { KeyCode } from "./.config/enums";

import { Samp } from "./includes/Samp";

while(true) {
    wait(0);
    if(!Samp.isAvailable()) continue;

    Samp.addChatMessage("SA:MP Cleo-Redux loaded", 0xFF0000);

    while(true) {
        wait(0);

        if(Pad.IsKeyDown(KeyCode.End)) {
            Samp.addChatMessage("Pressed button \"END\"!", 0x00CC00);
        }
    }
}
```
