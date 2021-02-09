# <center> VARA-TTS: Non-Autoregressive Text-to-Speech Synthesis based on Very Deep VAE with Residual Attention </center>

<center> Anonymous submission </center>

## Abstract
This paper proposes VARA-TTS, a non-autoregressive (non-AR) end-to-end text-to-speech (TTS) model using a very deep Variational Autoencoder (VDVAE) with Residual Attention mechanism, which refines the textual-to-acoustic alignment layer-wisely. Hierarchical latent variables with different temporal resolutions from the VDVAE are used as queries for the residual attention module. By leveraging the coarse global alignment from previous attention layer as an extra input, the following attention layer can produce a refined version of alignment. This amortizes the burden of learning the textual-to-acoustic alignment among multiple attention layers and outperforms the use of only a single attention layer in robustness. An utterance-level speaking speed factor is computed by a jointly-trained speaking speed predictor, which takes the mean-pooled latent variables of the coarsest layer as input, to determine number of acoustic frames at inference. Experimental results show that VARA-TTS achieves slightly inferior speech quality to an AR counterpart Tacotron 2 but an order-of-magnitude speed-up at inference; and outperforms an analogous non-AR model, BVAE-TTS, in terms of speech quality. 

Source Codes will be released soon!  

## Multi-speaker TTS (Chinese)

## Single-speaker TTS (English)

Text: Once held by Hobson and Dewey, now carried by Mother Eddy and Brother Dowie.

| **Tacotron 2** | **BVAE-TTS** | **VARA-TTS (ours)** |
| :--- | :--- | :--- |
| <audio src="wavs/en/taco2/121_121726_000025_000001.wav" controls preload></audio> | <audio src="wavs/en/bvae/121_121726_000025_000001.wav" controls preload></audio> | <audio src="wavs/en/vara/121_121726_000025_000001.wav" controls preload></audio> |
| --- | --- | --- |

Text: If the child gives the effect another turn of the screw, what do you say to TWO children?

| **Tacotron 2** | **BVAE-TTS** | **VARA-TTS (ours)** |
| :--- | :--- | :--- |
| <audio src="wavs/en/taco2/121_127105_000008_000002.wav" controls preload></audio> | <audio src="wavs/en/bvae/121_127105_000008_000002.wav" controls preload></audio> | <audio src="wavs/en/vara/121_127105_000008_000002.wav" controls preload></audio> |
| --- | --- | --- |

Text: But Polly couldn't speak; and if Jasper hadn't caught her just in time, she would have tumbled over backward from the stool, Phronsie and all!

| **Tacotron 2** | **BVAE-TTS** | **VARA-TTS (ours)** |
| :--- | :--- | :--- |
| <audio src="wavs/en/taco2/237_126133_000023_000000.wav" controls preload></audio> | <audio src="wavs/en/bvae/237_126133_000023_000000.wav" controls preload></audio> | <audio src="wavs/en/vara/237_126133_000023_000000.wav" controls preload></audio> |
| --- | --- | --- |


Text: "But," I remarked, "since we have followed the road that Saknussemm has shown us."

| **Tacotron 2** | **BVAE-TTS** | **VARA-TTS (ours)** |
| :--- | :--- | :--- |
| <audio src="wavs/en/taco2/260_123286_000016_000000.wav" controls preload></audio> | <audio src="wavs/en/bvae/260_123286_000016_000000.wav" controls preload></audio> | <audio src="wavs/en/vara/260_123286_000016_000000.wav" controls preload></audio> |
| --- | --- | --- |

Text: Such is their ponderous weight that they cannot rise from the horizon; but, obeying an impulse from higher currents, their dense consistency slowly yields.

| **Tacotron 2** | **BVAE-TTS** | **VARA-TTS (ours)** |
| :--- | :--- | :--- |
| <audio src="wavs/en/taco2/260_123288_000006_000002.wav" controls preload></audio> | <audio src="wavs/en/bvae/260_123288_000006_000002.wav" controls preload></audio> | <audio src="wavs/en/vara/260_123288_000006_000002.wav" controls preload></audio> |
| --- | --- | --- |

Text: We were on the edge of the Casanova churchyard.

| **Tacotron 2** | **BVAE-TTS** | **VARA-TTS (ours)** |
| :--- | :--- | :--- |
| <audio src="wavs/en/taco2/533_1066_000015_000004.wav" controls preload></audio> | <audio src="wavs/en/bvae/533_1066_000015_000004.wav" controls preload></audio> | <audio src="wavs/en/vara/533_1066_000015_000004.wav" controls preload></audio> |
| --- | --- | --- |


Text: O life of this our spring! why fades the lotus of the water? Why fade these children of the spring?

| **Tacotron 2** | **BVAE-TTS** | **VARA-TTS (ours)** |
| :--- | :--- | :--- |
| <audio src="wavs/en/taco2/908_157963_000010_000000.wav" controls preload></audio> | <audio src="wavs/en/bvae/908_157963_000010_000000.wav" controls preload></audio> | <audio src="wavs/en/vara/908_157963_000010_000000.wav" controls preload></audio> |
| --- | --- | --- |

Text: A ring of amethyst I could not wear here, plainer to my sight, Than that first kiss.

| **Tacotron 2** | **BVAE-TTS** | **VARA-TTS (ours)** |
| :--- | :--- | :--- |
| <audio src="wavs/en/taco2/908_31957_000017_000001.wav" controls preload></audio> | <audio src="wavs/en/bvae/908_31957_000017_000001.wav" controls preload></audio> | <audio src="wavs/en/vara/908_31957_000017_000001.wav" controls preload></audio> |
| --- | --- | --- |

Text: For a full hour he had paced up and down, waiting: but he could wait no longer.

| **Tacotron 2** | **BVAE-TTS** | **VARA-TTS (ours)** |
| :--- | :--- | :--- |
| <audio src="wavs/en/taco2/1089_134691_000002_000002.wav" controls preload></audio> | <audio src="wavs/en/bvae/1089_134691_000002_000002.wav" controls preload></audio> | <audio src="wavs/en/vara/1089_134691_000002_000002.wav" controls preload></audio> |
| --- | --- | --- |

Text: For a long time he had wished to explore the beautiful Land of Oz in which they lived.

| **Tacotron 2** | **BVAE-TTS** | **VARA-TTS (ours)** |
| :--- | :--- | :--- |
| <audio src="wavs/en/taco2/1284_1180_000006_000002.wav" controls preload></audio> | <audio src="wavs/en/bvae/1284_1180_000006_000002.wav" controls preload></audio> | <audio src="wavs/en/vara/1284_1180_000006_000002.wav" controls preload></audio> |
| --- | --- | --- |


