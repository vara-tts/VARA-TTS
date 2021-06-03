# <center> VARA-TTS: Non-Autoregressive Text-to-Speech based on Very Deep VAE with Residual Attention </center>

<center> Anonymous submission </center>

## Abstract
Non-autoregressive (non-AR) text-to-speech (TTS) models usually contain a separate phoneme-level duration predictor, which is trained with the supervision signal generated during training or from an external aligner. This paper proposes VARA-TTS, a non-AR TTS model using a very deep Variational Autoencoder (VDVAE) with Residual Attention mechanism, which refines the textual-to-acoustic alignment layer-wisely. Hierarchical representations with different temporal resolutions from the VDVAE are used as queries for the residual attention module. By leveraging coarse global alignment from the precedent attention layer, the descendant attention layer can produce a refined version. This coarse-to-fine mechanism distributes the burden of learning the textual-to-acoustic alignment into multiple attention layers, leading to more robust generation at inference. An utterance-level speaking speed factor is computed by a jointly-trained speaking speed predictor to determine the number of acoustic frames at inference. Experimental results show that VARA-TTS achieves similar speech quality to an AR counterpart Tacotron 2 but an order-of-magnitude speed-up at inference; and outperforms analogous non-AR models, Glow-TTS and BVAE-TTS, in terms of speech quality.

## Multi-speaker TTS (Chinese)

Text: 他怎么也该留下一只让我尝尝才是呀!

<audio src="wavs/zh/mig_feifei_820691.wav" controls preload></audio>

Text: 我回家传照片去了,请你告诉我,凤琴的号码。

<audio src="wavs/zh/tx_daji_000866.wav" controls preload></audio>

Text: 李元芳大招清一波线。

<audio src="wavs/zh/tx_guiniang_917000711.wav" controls preload></audio>

Text: 据伦敦北区消防队的官员说,摩总统主张摩加入独联体。

<audio src="wavs/zh/tx_daji_000591.wav" controls preload></audio>

Text: 出租车里电台广告都有宣传广告,大厦财大气粗啊!

<audio src="wavs/zh/mig_feifei_820258.wav" controls preload></audio>

Text: 我在外面,随便吃点就好了。

<audio src="wavs/zh/tx_daji_000906.wav" controls preload></audio>

Text: 曹操还是有一技能三段位移的。

<audio src="wavs/zh/tx_guiniang_917000739.wav" controls preload></audio>

Text: 十年沧海,劈波斩浪。

<audio src="wavs/zh/bb_fky_000364.wav" controls preload></audio>

Text: 广东省政协常委陈缵光走进“蚁族”居所。

<audio src="wavs/zh/bb_fky_000182.wav" controls preload></audio>

Text: 在该超市的促销海报上,双汇肘花火腿”也赫然在列。

<audio src="wavs/zh/bb_fky_000825.wav" controls preload></audio>

## Single-speaker TTS (English)

Text: the latter raised eighteen pence among them to pay for a truss of straw for the poor woman to lie on.

<audio src="wavs/en/vara/LJ002-0289.wav" controls preload></audio>

Text: They were never left quite alone for fear of suicide, and for the same reason they were searched for weapons or poisons.

<audio src="wavs/en/vara/LJ003-0211.wav" controls preload></audio>

Text: provided only that their security was not jeopardized, and dependent upon the enforcement of another new rule,

<audio src="wavs/en/vara/LJ003-0319.wav" controls preload></audio>

Text: One of the earliest of the big operators in fraudulent finance was Edward Beaumont Smith,

<audio src="wavs/en/vara/LJ013-0005.wav" controls preload></audio>

Text: with the idea of subjecting her to the irritant poison slowly but surely until the desired effect, death, was achieved.

<audio src="wavs/en/vara/LJ017-0164.wav" controls preload></audio>

Text: was to be the rule for all convicted prisoners throughout the early stages of their detention;

<audio src="wavs/en/vara/LJ019-0318.wav" controls preload></audio>

Text: Every facility was promised. The sanction of the Secretary of State would not be withheld if plans and estimates were duly submitted,

<audio src="wavs/en/vara/LJ019-0348.wav" controls preload></audio>

Text: treated the gunshot wound in the left thigh.

<audio src="wavs/en/vara/LJ031-0122.wav" controls preload></audio>

Text: He admitted to fantasies about being powerful and sometimes hurting and killing people, but refused to elaborate on them.

<audio src="wavs/en/vara/LJ040-0176.wav" controls preload></audio>

Text: as to the fact that he was an outstanding man, end quote.

<audio src="wavs/en/vara/LJ045-0092.wav" controls preload></audio>
