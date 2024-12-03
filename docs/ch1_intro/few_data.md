#### Motivation for Low Data Approaches

Deep learning models for beat and downbeat tracking have achieved remarkable success in recent years, but their effectiveness relies heavily on large amounts of annotated training data. This presents a significant challenge when applying these models to underrepresented music traditions, such as Latin American genres, where annotated datasets are often scarce. Annotating such data requires culturally informed expertise and substantial time investment, making large-scale data collection impractical. However, the rhythmic and metrical homogeneity observed in many traditional Latin American music styles, such as samba and candombe, suggests that beat tracking models might perform well with minimal annotated data. This section discusses the ideas behind this.

```{note}
The content in this section draws heavily from the following ISMIR 2022 publication from Maia et al.:
[`Adapting Meter Tracking Models to Latin American Music`](https://ismir2022program.ismir.net/poster_272.html)
```

---

#### When Can We Use Low Data?

In the context of beat tracking, low-data approaches seem to be most effective in musical contexts where:

1. **High Rhythmic Homogeneity**: The target music genre exhibits consistent rhythmic patterns, instrumentation, and tempos.
2. **Focused Applications**: The goal is to specialize a model for a specific subset of music, rather than creating a universal solution (i.e. a model that works for multiple genres).
3. **Limited Annotation Resources**: Only a few minutes of annotated audio are available, which is common in underrepresented or culturally-specific music genres.

For example, Samba and Candombe demonstrate rhythmic regularities that make them suitable candidates for such adaptations. On top of that, Candombe has fixed instrumentation, making it even more homogenious. 

---

#### How do we do it? Fine-Tuning vs. Training from Scratch

We explore to strategies to adapt beat tracking models with minimal data:

1. **Training from Scratch (TCN-FS)**: Models trained exclusively on the small, annotated dataset of the target genre. This approach benefits from rhythmic homogeneity but can struggle with generalization if the dataset is too small.
   
2. **Fine-Tuning Pretrained Models (TCN-FT)**: Transfer learning is employed to adapt a model initially trained on diverse Western music datasets. By fine-tuning on the small target dataset, the model leverages its pre-existing knowledge while specializing in the new domain. This strategy has shown better performance and faster convergence compared to training from scratch.