HeaderWriter
====

Just generates a WAVE-file header, with the specified length as argument.

```javascript
var header = require("waveheader");
//write to a normal fs.createWriteStream
myFileStream.write(header(44100 * 8)); // 44100 khz * 8 seconds


// using options (all available options listed)
myOtherFileStream.write(header(22050 * 8) {
  sampleRate: 22050,
  channels: 2,
  bitDepth: 8
}); 
