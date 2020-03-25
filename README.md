# RemoveOpenWithVisualStudioOnGitHub
No one needed this. At least make it look nice. Or just remove it.

```javascript
// ==UserScript==
// @name         Remove "Open With Visual Studio"
// @namespace    https://eric.golde.org/
// @version      1.0
// @description  Removes the shitty "Open with Visual Studio" button on Github. No one needs this. No one asked for this. At least make it look less shitty!!!
// @author       Eric Golde
// @match        https://github.com/*
// @grant        none
// ==/UserScript==

(function() {
    'use strict';
    try {
        document.querySelectorAll('[data-open-app]')[0].remove();
    }
    catch(err){
        //ignored.
    }
})();
```
