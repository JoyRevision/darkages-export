# Export

When the export is finished, add this segment of code to the JavaScript to capture the mouse properly:

```JavaScript
const canvas = document.getElementById('canvas');
canvas.addEventListener('click', async() => {
    await canvas.requestPointerLock();
});
```