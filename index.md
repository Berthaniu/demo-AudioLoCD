# <center> SoundLoCD: An Efficient Conditional Discrete Contrastive Latent Diffusion Model for Text-to-Sound Generation </center>

<center> Xinlei Niu<sup>1</sup>, Jing Zhang<sup>1</sup>, Christian Walder<sup>2</sup>, Charles Patrick Martin<sup>1</sup> </center> 
 
<center> 1 Australian National University, Canberra, Australia </center>

<center> 2 Google DeepMind, Montreal, Canada</center>

## Abstract
We present the SoundLoCD, a novel text-to-sound generation framework, which incorporates a LoRA-based conditional discrete contrastive latent diffusion model. Unlike recent large-scale sound generation models, our method can be efficiently trained under limited computational resources. The integration of a contrastive learning strategy further enhances the connection between textual conditions and the generated outputs, resulting in coherent and high-fidelity performance. Our experiments demonstrate that SoundLoCD outperforms the baseline with greatly reduced computational resources. A comprehensive ablation study further validates the contribution of each component within the SoundLoCD.

## Architecture
<center><img src="Figure/AudioLoCD.png" width="80%" height="80%" /></center>


## The comprarison between generated sample by SoundLoCD, DiffSound[1] (baseline), and Ground Truth (Source audio)
<!-- ### The comprarison between generated sample by AudioLoCD, DiffSound[1] (baseline), and Ground Truth -->

| <center>Text description</center> | <center>SoundLoCD</center> | <center>Diffsound</center> |<center>Ground Truth</center>|
| :--- | :--- | :--- |
|Food is frying then a woman speaks|<audio src="sample1/AudioLoCD.wav" controls preload></audio>|<audio src="sample1/DiffSound.wav" controls preload></audio>|<audio src="sample1/GT.wav" controls preload></audio>|
|Mel-spectrograms|<img src="sample1/AudioLoCD_mel.png" width="60%" height="60%" />|<img src="sample1/DS_mel.png" width="60%" height="60%" />|<img src="sample1/GT_mel.png" width="60%" height="60%" />|

|Speaking following by laughing and clapping|<audio src="sample2/AudioLoCD2.wav" controls preload></audio>|<audio src="sample2/DiffSound.wav" controls preload></audio>|<audio src="sample2/GT.wav" controls preload></audio>|
|Mel-spectrograms|<img src="sample2/AudioLoCD_mel.png" width="60%" height="60%" />|<img src="sample2/DS_mel.png" width="60%" height="60%" />|<img src="sample2/GT_mel.png" width="60%" height="60%" />|

|A woman speaks as she rubs two objects together|<audio src="sample3/AudioLoCD.wav" controls preload></audio>|<audio src="sample3/DiffSound.wav" controls preload></audio>|<audio src="sample3/GT.wav" controls preload></audio>|
|Mel-spectrograms|<img src="sample3/AudioLoCD_mel.png" width="60%" height="60%" />|<img src="sample3/DS_mel.png" width="60%" height="60%" />|<img src="sample3/GT_mel.png" width="60%" height="60%" />|

|A series of light horn beeps is followed by a loud steam whistle|<audio src="sample4/AudioLoCD.wav" controls preload></audio>|<audio src="sample4/DiffSound.wav" controls preload></audio>|<audio src="sample4/GT.wav" controls preload></audio>|
|Mel-spectrograms|<img src="sample4/AudioLoCD_mel.png" width="60%" height="60%" />|<img src="sample4/DS_mel.png" width="60%" height="60%" />|<img src="sample4/GT_mel.png" width="60%" height="60%" />|

|An engine runs then a train horn sounds|<audio src="sample5/AudioLoCD.wav" controls preload></audio>|<audio src="sample5/DiffSound.wav" controls preload></audio>|<audio src="sample5/GT.wav" controls preload></audio>|
|Mel-spectrograms|<img src="sample5/AudioLoCD_mel.png" width="60%" height="60%" />|<img src="sample5/DS_mel.png" width="60%" height="60%" />|<img src="sample5/GT_mel.png" width="60%" height="60%" />|


|A baby cries and fusses, a woman speaks, and a man speaks|<audio src="sample6/AudioLoCD.wav" controls preload></audio>|<audio src="sample6/DiffSound.wav" controls preload></audio>|<audio src="sample6/GT.wav" controls preload></audio>|
|Mel-spectrograms|<img src="sample6/AudioLoCD_mel.png" width="60%" height="60%" />|<img src="sample6/DS_mel.png" width="60%" height="60%" />|<img src="sample6/GT_mel.png" width="60%" height="60%" />|


|Children cry and people talk|<audio src="sample7/AudioLoCD.wav" controls preload></audio>|<audio src="sample7/DiffSound.wav" controls preload></audio>|<audio src="sample7/GT.wav" controls preload></audio>|
|Mel-spectrograms|<img src="sample7/AudioLoCD_mel.png" width="60%" height="60%" />|<img src="sample7/DS_mel.png" width="60%" height="60%" />|<img src="sample7/GT_mel.png" width="60%" height="60%" />|


|A grown man speaks as water softly runs|<audio src="sample8/AudioLoCD.wav" controls preload></audio>|<audio src="sample8/DiffSound.wav" controls preload></audio>|<audio src="sample8/GT.wav" controls preload></audio>|
|Mel-spectrograms|<img src="sample8/AudioLoCD_mel.png" width="60%" height="60%" />|<img src="sample8/DS_mel.png" width="60%" height="60%" />|<img src="sample8/GT_mel.png" width="60%" height="60%" />|

### References

[1] Yang, Dongchao, et al. "Diffsound: Discrete diffusion model for text-to-sound generation." IEEE/ACM Transactions on Audio, Speech, and Language Processing (2023).