```js
(function (length, c) {
    Array.from({ length }, (_, i) => i + 1)
        .map(e => c.repeat(e).padStart(length, '\u0020') + c.repeat(e - 1))
        .concat(Array.from({ length: length / 3 }, (_, i) => i + 1)
            .map(() => c.repeat(length / 3).padStart(length + length / 7, '\u0020')))
        .concat(' __  __                       __  __     __  __           ')
        .concat('|  \\/  | ___ _ __ _ __ _   _  \\ \\/ /    |  \\/  | __ _ ___ ')
        .concat('| |\\/| |/ _ \\ \'__| \'__| | | |  \\  /_____| |\\/| |/ _` / __|')
        .concat('| |  | |  __/ |  | |  | |_| |  /  \\_____| |  | | (_| \\__ \\')
        .concat('|_|  |_|\\___|_|  |_|   \\__, | /_/\\_\\    |_|  |_|\\__,_|___/')
        .concat('                       |___/                              ')
        .forEach(_ => console.log(_));
})(0x2A >> 1, '\u002A')
```
