# itunes-control
control iTunes with node

## install
  
  npm install --save itunes-control
  
## usage

```js
var iTunes = require('itunes-control');

iTunes.createPlaylist('fav', function (err) {
  if (err) {
    return;
  }
  iTunes.addToPlaylist('fav', './song.mp3');
})
```


## API

There only two methods so far

`iTunes.createPlaylist(<playlist-name>, <callback>);`

`iTunes.addToPlaylist(<playlist-name>, <filename>, <callback>);`
