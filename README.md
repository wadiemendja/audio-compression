# audio-compression

Audio compression is data compression designed to reduce the transmission bandwidth requirement of digital audio streams and the storage size of audio files. Broadly compression techniques are classified into two types:
Lossless compression algorithms usually exploit statistical redundancy in such a way as to represent the sender's data more concisely without error. Lossless compression schemes are reversible so that the original data can be reconstructed
Lossy schemes accept some loss of data in order to achieve higher compression.

In both lossy and lossless compression, information redundancy is reduced, using methods such as coding, pattern recognition and linear prediction to reduce the amount of information used to represent the uncompressed data.

There are numerous methods of compressing audio files. The Discrete Cosine Transform is a lossy technique that removes certain frequencies from the audio data such that the size is reduced with reasonable quality.

The Discrete Cosine Transform is a first-level approximation to mpeg audio compression, which are more sophisticated forms of the basic principle used in DCT.

This discrete cosine Transform Audio Compression is performed in  MATLAB.

It takes a wave file as input, compress it to different levels and assess the output that is each compressed wave file. The difference in their frequency spectra will be viewed to assess how different levels of compression affect the audio signals.

PROGRAM WORKING:-

An audio waveform is a continuous sequence of data in one long vector. In that sense, an audio data structure is different from an image data structure. We will need to apportion the vector manually into several pieces, and cannot rely on existing rows or columns.
Read the audio file
Determine a value for the number of samples that will undergo a DCT at once. In other words, the audio vector will be divided into pieces of this length.
Again, we examine at different compression rates:

50%
75%
87.5%
Resulting compressed-and-uncompressed audio waves

For simplicity, we iterate over the vector, window-by-window, but we discard whatever remainder exists:
Now we plot the time domain signals

![alt text](/Capture.PNG)

However, closer inspection does reveal qualitative differences in the densely packed regions (high frequencies).
A look at the spectrogram reveals a clear idea of the loss of high frequencies.

![alt text](/Capture2.PNG)

The qualitative difference is clearly apparent when listening to the audio files
Saving the files and viewing the difference in size


CODE

%read a file and convert it to a vector

%chosing a block size

%changing compression  percentages

%initializing compressed matrice

%actual compression

%plotting audio signals

%expanded view of audio signals

%spectrogram of audio signals

%playing files
