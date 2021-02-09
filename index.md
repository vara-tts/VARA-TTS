# <center> VARA-TTS: Non-Autoregressive Text-to-Speech Synthesis based on Very Deep VAE with Residual Attention </center>

<center> Anonymous submission </center>

## Abstract
This paper proposes VARA-TTS, a non-autoregressive (non-AR) end-to-end text-to-speech (TTS) model using a very deep Variational Autoencoder (VDVAE) with Residual Attention mechanism, which refines the textual-to-acoustic alignment layer-wisely. Hierarchical latent variables with different temporal resolutions from the VDVAE are used as queries for the residual attention module. By leveraging the coarse global alignment from previous attention layer as an extra input, the following attention layer can produce a refined version of alignment. This amortizes the burden of learning the textual-to-acoustic alignment among multiple attention layers and outperforms the use of only a single attention layer in robustness. An utterance-level speaking speed factor is computed by a jointly-trained speaking speed predictor, which takes the mean-pooled latent variables of the coarsest layer as input, to determine number of acoustic frames at inference. Experimental results show that VARA-TTS achieves slightly inferior speech quality to an AR counterpart Tacotron 2 but an order-of-magnitude speed-up at inference; and outperforms an analogous non-AR model, BVAE-TTS, in terms of speech quality. 

Source Codes will be released soon!  

## Single-speaker TTS

1. Text: Once held by Hobson and Dewey, now carried by Mother Eddy and Brother Dowie.
| **Tacotron 2** | **BVAE-TTS** | **VARA-TTS (ours)** |
| :--- | :--- | :--- |
| <audio src="wavs/recordings/clb/arctic_a0015.wav" controls preload></audio> | <audio src="wavs/recordings/clb/arctic_a0015.wav" controls preload></audio> | <audio src="wavs/recordings/clb/arctic_a0015.wav" controls preload></audio> |
| --- | --- | --- | --- | --- | --- |
