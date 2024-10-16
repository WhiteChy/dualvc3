# dualvc3
replicate

1、content encoder (Dynamic Chunk Training) wenet conformerencoder [link]([https://github.com/jik876/hifi-gan](https://github.com/wenet-e2e/wenet/blob/main/wenet/transformer/encoder.py#L440))

2、hifigan causal training [link](https://github.com/jik876/hifi-gan)

3、hpc loss ([apc](https://github.com/iamyuanchung/Autoregressive-Predictive-Coding) and [cpc](https://github.com/Spijkervet/contrastive-predictive-coding))

4、wav2vec2.0 cross entropy loss

I refer to [link](https://github.com/facebookresearch/fairseq/tree/main/examples/hubert/simple_kmeans) to implement kmeans clusters

5、gumbel softmax 

F.gumbel_softmax(x,t=1,hard=True)

6、llama training [llama](https://github.com/ypeleg/llama)

7、use pretrained speaker encoder [wespeaker](https://github.com/wenet-e2e/wespeaker)

8、wavaugment augmentation [wavaugment](https://github.com/facebookresearch/WavAugment)

9、llama and decoder combination **ing**
