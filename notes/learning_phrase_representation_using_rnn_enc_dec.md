# Learning Phrase Representations using RNN Encoder-Decoder for Statistical Machine Translation

</br>

#### Contributions

They propose a novel neural network model called RNN Encoder-Decoder that learns to encode a input sequence of variable-length into a fixed-length vector representation and to decode the vector representation back into a variable-length sequence.

In addition to novel neural network architecture, they propose a new type of activation unit called GRU which has been motivated by the LSTM unit but is much simpler to compute and implement.



#### Notes

As can be seen in Figure 1, They use skip connections when compute the conditional distribution of the next symbol. 

(Figure 2) In GRU, if update gate == 1 then previous hidden state is propagated to current hidden state. If update gate == 0 and reset gate == 0 then model is forced to ignored previous hidden state and reset with current input only. 


#### Future Work

The performance of the proposed model deteriorates rapidly as the length of an input sequence increases. This is because the model needs to be able to compress all the necessary information of a source sentence into a fixed-length vector. Dzmitry Bahdanau et al. <b>Neural Machine Translation by Jointly Learning to Align and Translate</b> conjecture this problem and propose to extend this by allowing a model to automatically search for parts of a source sentence that are relevant to predicting a target word (soft attention).

