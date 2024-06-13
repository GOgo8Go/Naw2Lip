Highlights

    Weights of the visual quality disc has been updated in readme!
    Lip-sync videos to any target speech with high accuracy 💯. Try our interactive demo.
    ✨ Works for any identity, voice, and language. Also works for CGI faces and synthetic voices.
    Complete training code, inference code, and pretrained models are available 💥
    Or, quick-start with the Google Colab Notebook: Link. Checkpoints and samples are available in a Google Drive folder as well. There is also a tutorial video on this, courtesy of What Make Art. Also, thanks to Eyal Gruss, there is a more accessible Google Colab notebook with more useful features. A tutorial collab notebook is present at this link.
    🔥 🔥 Several new, reliable evaluation benchmarks and metrics [evaluation/ folder of this repo] released. Instructions to calculate the metrics reported in the paper are also present.
The result is saved (by default) in results/result_voice.mp4. You can specify it as an argument, similar to several other available options. The audio source can be any file supported by FFMPEG containing audio data: *.wav, *.mp3 or even a video file, from which the code will automatically extract the audio.
Tips for better results:

    Experiment with the --pads argument to adjust the detected face bounding box. Often leads to improved results. You might need to increase the bottom padding to include the chin region. E.g. --pads 0 20 0 0.
    If you see the mouth position dislocated or some weird artifacts such as two mouths, then it can be because of over-smoothing the face detections. Use the --nosmooth argument and give it another try.
    Experiment with the --resize_factor argument, to get a lower-resolution video. Why? The models are trained on faces that were at a lower resolution. You might get better, visually pleasing results for 720p videos than for 1080p videos (in many cases, the latter works well too).
    The Wav2Lip model without GAN usually needs more experimenting with the above two to get the most ideal results, and sometimes, can give you a better result as well.
