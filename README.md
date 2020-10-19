# pyffmpeg    ![Travis (.org)](https://img.shields.io/travis/deuteronomy-works/pyffmpeg/build-linux?label=Linux&logo=linux&logoColor=white&style=for-the-badge)  ![Travis (.org)](https://img.shields.io/travis/deuteronomy-works/pyffmpeg/build-darwin?label=MacOs&logo=apple&style=for-the-badge)  ![Travis (.org)](https://img.shields.io/travis/deuteronomy-works/pyffmpeg/build-windows?label=Windows&logo=windows&style=for-the-badge)  [![Downloads](https://pepy.tech/badge/pyffmpeg)](https://pepy.tech/project/pyffmpeg)


FFmpeg wrapper for python.

The beautiful thing about it is that it comes with its own FFmpeg executable. It is compressed, making it the smallest you can find. And becuase its cross-platform and python 3, it is the only option available for building cross-platform apps with ffmpeg in python.

## Installation
    pip install pyffmpeg

## Usage
### FFmpeg
```python
from pyffmpeg import FFmpeg

inp = 'path/to/music_folder/f.mp4'
out = 'path/to/music_folder/f.mp3'

ff = FFmpeg()

output_file = ff.convert(inp, out)

print(output_file)

```

### FFprobe
Provides FFprobe functions and values

## Usage
### import statement
```python
from pyffmpeg import FFprobe

input_file = 'path/to/music.mp3'
fp = FFprobe(input_file)
```

The probing is done when the class is called this way. The object now
contains the various values stored under their names eg

```python
print(fp.duration)
```
will print
```shell
> 00:04:32:32
```
NB: The above is just for illustration


## Wiki
The wiki can be located [here](https://github.com/deuteronomy-works/pyffmpeg/wiki)
