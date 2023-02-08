# fastClusteringDiarizer: fast clustering of speaker embeddings for multifile speaker diarization with reappearing speakers

## About

Speaker diarization is the process of identifying speakers in a recording and assigning them to a speaker cluster. 

However, analysis of audio data often involves the identification of speakers across multiple recordings in order to create speaker-aware transcripts, e.g. for work meetings, interviews, lectures, or podcasts. In these cases, it is desirable to have a speaker diarization system that can natively handle multiple recordings and reappearing speakers. In this repository, I present a speaker diarization pipeline that handles the challenges of this task.
These challenges include:
- Speaker embeddings extracted from multiple recordings might not be comparable, due to differences in recording conditions, e.g. microphone, background noise, etc.
- Speakers might appear in multiple recordings
- New speakers might get introduced in later recordings

Audio data originates from a free access, Hungarian language podcast. More info [in this repo](https://github.com/bghorvath/filmbaradatok).
Speaker embeddings were extracted using the pyannote.audio framework and a speechbrain speaker embedding model.
Agglomerative clustering method was used for the cluster data.
