
# Neural Machine Translation by Jointly Learning to Align and Translate
RNN Encoder-Decoder model which is proposed in Kyunghyun Cho et al. <b>Learning Phrase Representations using RNN Encoder-Decoder for Statistical Machine Translation
</b> encodes a source sequence of variable-length into a fixed-length vector representation and decodes the vector representation into a 
target sequence of variable-length. 

In this paper, they conjecture that the use of a fixed-length vector is a bottleneck in improving the performance of RNN Encoder-Decoder architecture and
propose to extend this by allowing the model to automatically search for parts of a source sequence that are relevant to predicting a target 
sequence.


### Contributions

They proposed a novel neural network model which uses soft attention to select adaptively parts of a source sequence.

They achieved a translation preformance comparable to the existing state-of-the-art phrase-based system on the task of English-to-French
translation.
