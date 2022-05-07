
# Laion - the big plan

**Overarching goal:** Enable the open source community to openly build datasets, papers, models and tools in order to let AGI benefit humankind even faster.

## Intro

Laion was initiated with the Laion5B project that successfully produced a 5B (image, text) pairs dataset by processing commoncrawl and filtering with clip. That method proved that it’s cheap to collect large scale dataset from the web using models like clip that give the similarity between items from 2 modalities.

Many models have been trained on laion400m proving the value of this method, with in particular openclip that reproduced the same results that the initial openai clip.

Let’s reproduce that method to **more modalities**!

## Directions

Methods

* Open source: releasing everything openly
  * Code: on github with an open license
  * Model: freely distributed models
  * Dataset: freely distributed datasets
* Open development: development is done in public on github and discord, everyone is encouraged to participate, whatever their nationality, age and diploma

Axis of work:

* Open tools
  * Dataset collection
  * Dataset preparation
  * Distributed inference
  * Distributed training
  * Evaluation
* Datasets
  * Open distribution
  * Papers
* Models
  * Open training
  * Open distribution

Scientific domains

* All modalities dataset building
  * Text image
  * Text audio
  * Text video
  * Text 3d
* Contrastive and generative
  * Contrastive
    * Text image
    * Text audio
    * Text video
  * Generative
    * Text to image
    * Image to text

## Projects

These projects are collaborations between many people. If you want to know who, check the links and ask in discord. We are open to new collaborators!

### Dataset

<table>
  <tr>
   <td>Name
   </td>
   <td>Modality
   </td>
   <td>Status
   </td>
   <td>Notes
   </td>
  </tr>
  <tr>
   <td><a href="https://laion.ai/laion-400-open-dataset/">Laion400m</a>
   </td>
   <td>image/text
   </td>
   <td>Done
   </td>
   <td>> 10 papers using it
   </td>
  </tr>
  <tr>
   <td><a href="https://laion.ai/laion-5b-a-new-era-of-open-large-scale-multi-modal-datasets/">Laion5B</a>
   </td>
   <td>image/text
   </td>
   <td>Done
   </td>
   <td>Largest open text/image dataset
   </td>
  </tr>
  <tr>
   <td><a href="https://huggingface.co/datasets/laion/laion-high-resolution">Laion5B high-resolution</a>
   </td>
   <td>image/text
   </td>
   <td>Done
   </td>
   <td>Largest open high-resolution text/image dataset
   </td>
  </tr>
  <tr>
   <td><a href="https://huggingface.co/datasets/laion/balanced-laion5b">Laion5B balanced</a>
   </td>
   <td>image/text
   </td>
   <td>Just started
   </td>
   <td>Balanced LAION-5B dataset for more efficient training
   </td>
  </tr>
  <tr>
   <td><a href="https://github.com/LAION-AI/laion-3d">laion3d</a>
   </td>
   <td>3d/image/text
   </td>
   <td>Just started
   </td>
   <td>Trying to expand the laion idea to 3d
   </td>
  </tr>
  <tr>
   <td><a href="https://github.com/LAION-AI/audio-dataset">Audio dataset</a>
   </td>
   <td>text/audio
   </td>
   <td>Started
   </td>
   <td>Started to be used to train an audio clip
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
</table>

### Model

<table>
  <tr>
   <td>Name
   </td>
   <td>Modality
   </td>
   <td>Kind
   </td>
   <td>Status
   </td>
   <td>Notes
   </td>
  </tr>
  <tr>
   <td><a href="https://github.com/mlfoundations/open_clip">Openclip B/16</a>
   </td>
   <td>image/text
   </td>
   <td>contrastive
   </td>
   <td>released
   </td>
   <td>Reproduced openai clip
   </td>
  </tr>
  <tr>
   <td><a href="https://github.com/lucidrains/DALLE2-pytorch">Dalle2 prior/decoder</a>
   </td>
   <td>image/text
   </td>
   <td>generative
   </td>
   <td>Just started
   </td>
   <td>Trying to reproduce dalle2
   </td>
  </tr>
  <tr>
   <td><a href="https://github.com/TheoCoombes/ClipCap">Clipcap</a>
   </td>
   <td>image/text
   </td>
   <td>generative
   </td>
   <td>works
   </td>
   <td>Generate text from embedding
   </td>
  </tr>
  <tr>
   <td>Audio clip
   </td>
   <td>audio/text
   </td>
   <td>contrastive
   </td>
   <td>Training on going
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><a href="https://github.com/LAION-AI/video-clip">Video clip</a>
   </td>
   <td>video/text
   </td>
   <td>contrastive
   </td>
   <td>Just started
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><a href="https://github.com/FreddeFrallan/Multilingual-CLIP">Mclip vit-l/14</a>
   </td>
   <td>image/text
   </td>
   <td>contrastive
   </td>
   <td>Just started
   </td>
   <td>Aligning a text encoder to be in clip space. Collaboration with mclip author
   </td>
  </tr>
  <tr>
   <td><a href="https://github.com/LAION-AI/super-resolution">Super-resolution</a>
   </td>
   <td>image->image
   </td>
   <td>generative
   </td>
   <td>Just started
   </td>
   <td>Using a high-resolution subset of LAION-5B for the training
   </td>
  </tr>
    <tr>
   <td><a href="https://github.com/LAION-AI/medical">Medical CLIP</a>
   </td>
   <td>image/text
   </td>
   <td>contrastive
   </td>
   <td>Just started
   </td>
   <td>Using CLIP to improve MRI -> image synthesis (see project outline).
   </td>
  </tr>
    <tr>
   <td><a href="https://github.com/LAION-AI/CLIP-based-NSFW-Detector">NSFW detection</a>
   </td>
   <td>image/text
   </td>
   <td>contrastive
   </td>
   <td>Done
   </td>
   <td>Using CLIP to detect NSFW in images.
   </td>
  </tr>
      <tr>
   <td><a href="https://github.com/LAION-AI/LAION-5B-WatermarkDetection">Watermark detection</a>
   </td>
   <td>image/text
   </td>
   <td>contrastive
   </td>
   <td>Done
   </td>
   <td>Using CLIP to detect watermarks in images.
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
</table>

### Tools

<table>
  <tr>
   <td>Name
   </td>
   <td>Modality
   </td>
   <td>Status
   </td>
   <td>Notes
   </td>
  </tr>
  <tr>
   <td><a href="https://github.com/rom1504/img2dataset">img2dataset</a>
   </td>
   <td>image/text
   </td>
   <td>working
   </td>
   <td>Used to download laion5B in a week, twice
   </td>
  </tr>
  <tr>
   <td><a href="https://github.com/rom1504/clip-retrieval">Clip retrieval</a>
   </td>
   <td>image/text
   </td>
   <td>working
   </td>
   <td>Used to compute 5B Vit-L/14 embeddings
   </td>
  </tr>
  <tr>
   <td><a href="https://github.com/rvencu/crawlingathome-gpu-hcloud">Crawlingathome-gpu-hcloud </a>
   </td>
   <td>image/text
   </td>
   <td>done
   </td>
   <td>Filtering common crawl using clip
   </td>
  </tr>
  <tr>
   <td><a href="https://github.com/LAION-AI/CLIP_benchmark">clip benchmark</a>
   </td>
   <td>image/text
   </td>
   <td>wip
   </td>
   <td>Evaluating clip performances easily
   </td>
  </tr>
</table>


### Papers

<table>
  <tr>
   <td>Name
   </td>
   <td>Modality
   </td>
   <td>Status
   </td>
   <td>Notes
   </td>
  </tr>
  <tr>
   <td><a href="https://arxiv.org/abs/2111.02114">Laion400m</a>
   </td>
   <td>image/text
   </td>
   <td>In arvix
   </td>
   <td>Cited many times
   </td>
  </tr>
  <tr>
   <td><a href="https://github.com/LAION-AI/laion5B-paper">laion5B</a>
   </td>
   <td>image/text
   </td>
   <td>started
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
</table>
