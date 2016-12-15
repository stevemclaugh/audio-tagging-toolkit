

Install dependencies:

```bash
pip install -i dependencies.txt
```
>Note: Let me know if this dependency list is incomplete: stephen.mclaughlin@utexas.edu

Install FFmpeg with MP3 support (at your own risk):

```bash
add-apt-repository -y ppa:mc3man/trusty-media
apt-get update
apt-get -y dist-upgrade
apt-get -y install ffmpeg
```

Locate applause in single file:

```bash
cd /path/to/audio-tagging-toolkit

python FindApplause.py -c -b -l "Speaker Name" -i /path/to/audio.mp3
```

Batch applause classification:

```bash
cd /path/to/audio-tagging-toolkit

python FindApplause.py -c -b -l "Speaker Name" path/to/directory/
```

Diarize a single file:

```bash
cd /path/to/audio-tagging-toolkit

python Diarize.py -b -c -i /Users/mclaugh/Desktop/attktest/Creeley-Robert_33_A-Note_Rockdrill-2.mp3
```

Batch Diarize:

```bash
cd /path/to/audio-tagging-toolkit

python Diarize.py -b -c /Users/mclaugh/Desktop/attktest/
```