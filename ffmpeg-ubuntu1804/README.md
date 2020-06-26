## How to Use

```bash
docker build -t ffmpeg-ubuntu .
mkdir tmp
mv test.wav tmp
```

### output input file's info

```bash
docker run -it --rm -v $PWD/tmp:/tmp/tmp ffmpeg-ubuntu:latest ffprobe /tmp/tmp/test.wav
```

### encode

```bash
docker run -it --rm -v $PWD/tmp:/tmp/tmp ffmpeg-ubuntu:latest ffmpeg -i /tmp/tmp/test.wav /tmp/tmp/output.avi
```
