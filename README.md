![image](https://github.com/user-attachments/assets/f330bdb6-05c7-4942-8e8f-4d3f39a8684d)# dualvc3
replicate

1、content encoder (Dynamic Chunk Training)  [wenet ConformerEncoder](https://github.com/wenet-e2e/wenet/blob/main/wenet/transformer/encoder.py#L440)

2、hifigan causal training [link](https://github.com/jik876/hifi-gan)

    y = torch.nn.functional.pad(y.unsqueeze(1), (int((n_fft-hop_size)), 0), mode='reflect')


3、hpc loss ([apc](https://github.com/iamyuanchung/Autoregressive-Predictive-Coding) and [cpc](https://github.com/Spijkervet/contrastive-predictive-coding))

4、wav2vec2.0 cross entropy loss

I refer to [link](https://github.com/facebookresearch/fairseq/tree/main/examples/hubert/simple_kmeans) to implement kmeans clusters

5、gumbel softmax 

F.gumbel_softmax(x,t=1,hard=True)

6、llama training [llama](https://github.com/ypeleg/llama)

7、use pretrained speaker encoder [wespeaker](https://github.com/wenet-e2e/wespeaker)

8、wavaugment augmentation [wavaugment](https://github.com/facebookresearch/WavAugment)

9、llama and decoder combination **ing**

10、use one future block for training **to do**

### results:
My replicated DualVC3 (stand-alone mode) have 20.164M params in inference without 1 chunk lookahead, which is twice than 10.9M (paper).
But it's performance is better than streamvc (1.7M params & 2 frame look ahead).
