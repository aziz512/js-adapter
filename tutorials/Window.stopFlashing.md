Stops the taskbar icon from flashing

# Example
```js
async function stopWindowFlashing() {
    const app = await fin.Application.start({
        name: 'myApp',
        uuid: 'app-1',
        url: 'https://cdn.openfin.co/docs/javascript/stable/tutorial-Window.stopFlashing.html',
        autoShow: true
    });
    const win = await app.getWindow();
    return await win.stopFlashing();
}

stopWindowFlashing().then(() => console.log('Application window flashing')).catch(err => console.log(err));
```
