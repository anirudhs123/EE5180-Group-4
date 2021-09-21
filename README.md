# Music Instrument Classification

In this project we use CNN based models to classify instruments using the Freesound audio data set. Our proposed architecture computes the Mel-spectrogram from the input audio
data and feeds it to a CNN based model. To add robustness to the model, we use a novel data augmentation technique based on the CutMix Algorithm. We optimise the architecture using Hyperparameter Tuning and Pruning, and analyse the model by generating the Class Activation Maps and by conducting an Ablation Study. For detailed information regarding this work, please read our detailed [report](https://emilbiju.github.io/indic-swipe). 

The models and datasets have been developed to cater to two closely related tasks:

- **Indic-to-Indic Decoding:** To support users who prefer to type in the native Indic script (Devanagari, Bengali, etc.)
- **English-to-Indic Decoding:** To support users who prefer to type using an English script keyboard but want the output in the native script.

IndicSwipe demonstrates high decoding accuracies on both tasks varying from 70% to 95% across the 7 languages.

<p align="center">
   <img src="../gh-pages/assets/images/gesture_sample.jpg" width=400 height=300>
</p>

## Key Contributions

1. A Gesture Path Decoding model that uses a multi-headed Transformer along with LSTM layers for coordinate sequence encoding and a character-level LSTM model for character sequence decoding.
2. A Contrastive Transliteration correction model that uses position-aware character embeddings to measure word proximities and correct spellings of transliterated words.
3. Two datasets of simulated word traces for supporting work on gesture typing for Indic language keyboards including low resource languages like Telugu and Kannada.
4. The accuracies of the proposed models vary from 70 to 89% for English-to-Indic decoding and 86-95% for Indic-to-Indic decoding across the 7 languages used for the study.

## People

This work has been developed as a part of a course project  by [Anirudh Sriram](https://github.com/anirudhs123), [Arjun Menon V], [Srinivas Mareddi] and [Nithin Varma] from the Indian Institute of Technology, Madras. Ask us your questions at [anirudhsriram30799@gmail.com](mailto:anirudhsriram30799@gmail.com).
