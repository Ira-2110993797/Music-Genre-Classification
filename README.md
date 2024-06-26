# Music-Genre-Classification


![Music](Assets/mgc.png)



# Overview
Music genre classification is a complex and fascinating task within the field of music information retrieval (MIR). It involves the automated categorization of music tracks into genres based on their audio features. This process leverages various techniques in machine learning and deep learning to analyze attributes such as tempo, rhythm, pitch, and timbre. Accurate genre classification can enhance music recommendation systems, improve user experience in music streaming services, and aid in organizing large music libraries.

The primary challenge in this domain is the diversity and variability in music, which includes differences in recording quality, instrumentation, and production styles. Additionally, obtaining a comprehensive and diverse dataset is crucial for training robust models. This project utilizes the Million Song Dataset (MSD), a large-scale collection of audio features and metadata for a million contemporary popular music tracks. By leveraging advanced machine learning algorithms and the MSD, this project aims to develop a reliable music genre classification system, addressing both the challenges of data acquisition and the complexity of musical diversity. Detailed documentation and scripts are provided to facilitate replication and further exploration.



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



![Music Genres](Assets/mg.jpeg)
