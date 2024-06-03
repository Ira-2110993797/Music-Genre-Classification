# Music-Genre-Classification


![Uploading image.png…]()



# Overview
Music genre classification is the task of automatically assigning a genre label to a piece of music. It plays a crucial role in various applications such as music recommendation systems, music search engines, and personalized playlists.



# Dataset
Acquiring the dataset was one of the most time-consuming aspects of this project. Working with music data is particularly challenging due to the large file sizes, varying recording qualities, and different parameters such as sampling rates and bit depths. The most significant challenge, however, is navigating copyright issues, as legitimate datasets of popular songs are often expensive and difficult to obtain. Tao's research utilized the GTZAN dataset, which comprises 100 songs per genre across 10 genres, totaling 1,000 songs. However, this dataset is relatively small, and its copyright status is uncertain, which likely hindered his results.

To address this, I sought a larger dataset and discovered the Million Song Dataset (MSD), a publicly available collection of audio features and metadata for a million contemporary popular music tracks, totaling approximately 280 GB of metadata. A related project, Tagtraum, classifies MSD songs into genres. The challenge then was to obtain the audio files themselves. I found that each song in the MSD dataset has an ID from a provider called 7Digital, a SaaS platform for music streaming. By registering as a developer with 7Digital and gaining API access, I discovered that they offer 30-second previews of songs for free before requiring payment. This preview duration was sufficient for my deep learning tasks. Consequently, I developed a script, "previewDownloader.py," to download 30-second previews for each song in the MSD dataset. Due to hardware limitations, I was only able to download previews for 1% of the dataset, amounting to approximately 2.8 GB.

The genres I am classifying are:

1. blues
2. classical
3. country
4. disco
5. hiphop
6. jazz
7. metal
8. pop
9. reggae
10. rock

Link for dataset: https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification
