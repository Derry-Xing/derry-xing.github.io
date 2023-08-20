1 July, 2022

# MVSPlenOctree: Fast and Generic Reconstruction of Radiance Fields in PlenOctree from Multi-view Stereo
 [Wenpeng Xing](https://Derry-Xing.github.io/)<sup>1</sup>,
 [Jie Chen](https://jchenhkg.github.io/)<sup>1</sup> <br>
 <sup>1</sup>Department of Computer Science, Hong Kong Baptist University  

### [Paper]() 

<br>

<div style="text-align: center"><img src="/projects/MVSPlenOctree/web/teaser.png" width="880"/></div>

<br>

### Abstract
* We present MVSPlenOctree, a novel approach that can efficiently reconstruct radiance fields for view synthesis.Unlike previous scene-specific radiance fields reconstruction methods, we present a generic pipeline that can efficiently reconstruct 360◦-renderable radiance fields via multi-view stereo (MVS) inference from tens of sparse-spread out images. Our approach leverages variance-based statistic features for MVS inference, and combines this with image based rendering and volume rendering for radiance field reconstruction. We first train a MVS Machine for reasoning scene’s density and appearance. Then, based on the spatial hierarchy of the PlenOctree and coarse-to-fine dense sampling mechanism, we design a robust and efficient sampling strategy for PlenOctree reconstruction, which handles occlusion robustly. A 360◦-renderable radiance fields can be reconstructed in PlenOctree from MVS Machine in an efficient single forward pass. We trained our method on real-world DTU, LLFF datasets, and synthetic datasets. We validate its generalizability by evaluating on the test set of DTU dataset which are unseen in training. In summary, our radiance field reconstruction method is both efficient and generic, a coarse 360◦-renderable radiance field can be reconstructed in seconds and a dense one within minutes.

<br>

### Pipeline
<div style="text-align: center"><img src="/projects/MVSPlenOctree/web/pipeline.png" width="780"/></div>

* The overall pipeline of MVSPlenOctree contains training stage and inference stage. The training stage trains a generic MVS Machine that outputs radiance fields through MVS, and can generalize to novel scenes. The inference stage is reconstructing radiance fields in PlenOctree by querying the pre-trained MVS Machine. The output PlenOctree data structure can be directly rendered in real-time.

<br>

### Video

<div style="text-align: center">
<iframe width="700" height="385" src="https://www.youtube.com/embed/yUtVphyYwLs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>



<br>

### Citation

```
@inproceedings{xingmvsplenoctree,
  title={MVSPlenOctree: Fast and Generic Reconstruction of Radiance Fields in PlenOctree from Multi-view Stereo},
  author={Wenpengxing, Jie Chen},
  year={2022},
  booktitle={Proceedings of the 30th ACM International Conference on Multimedia},
}
```

<div style="text-align: center">
<body width="10" height="10">
<script type='text/javascript' id='clustrmaps' src='//cdn.clustrmaps.com/map_v2.js?cl=140303&w=70&t=n&d=RcKt1V3_wR-r-8eU1oJP38UI1pbIxzDP91mIQUtDo78&co=ffffff'></script>
</body>
</div>


