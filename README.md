# helper_javascript
A collection of helper scripts for browser automation

Clear YouTube watchlist:

```
function clickFirstVideo() {
  document
    .querySelector('.style-scope ytd-playlist-video-renderer button')
    .click();
}

function clickDeleteButton() {
  document.querySelectorAll('ytd-menu-service-item-renderer')[2].click()
}

setInterval(() => {
  clickFirstVideo();
  clickDeleteButton();
}, 100);
```
