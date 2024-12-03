Beat tracking with little data
==============================================

---

#### Fine-Tuning vs. Training from Scratch

Two primary strategies were explored to adapt beat tracking models with minimal data:

1. **Training from Scratch (TCN-FS)**: Models trained exclusively on the small, annotated dataset of the target genre. This approach benefits from rhythmic homogeneity but can struggle with generalization if the dataset is too small.
   
2. **Fine-Tuning Pretrained Models (TCN-FT)**: Transfer learning is employed to adapt a model initially trained on diverse Western music datasets. By fine-tuning on the small target dataset, the model leverages its pre-existing knowledge while specializing in the new domain. This strategy has shown better performance and faster convergence compared to training from scratch.

---

#### Results

##### Performance

1. **Minimal Data Requirements**:
   - Models fine-tuned with as little as 1.5 minutes of annotated data achieved F-measure scores exceeding 80% for beat tracking in both samba and candombe.
   - Downbeat tracking performance showed similar trends, although samba required slightly more data to achieve comparable results due to its greater timbral and rhythmic complexity.

2. **Data Augmentation**:
   - Applying simple augmentation strategies, such as varying the input's tempo, significantly improved model performance, especially for downbeat tracking in samba.

3. **Comparative Analysis**:
   - Fine-tuned models with data augmentation (TCN-FTA) consistently outperformed models trained from scratch (TCN-FS) and statistical baselines like BayesBeat.
   - Off-the-shelf models trained on Western datasets performed poorly, highlighting the importance of cultural specificity in model adaptation.

##### Computational Cost

Training the fine-tuned model required minimal computational resources:
- Models trained with data augmentation on a standard CPU achieved near-full-dataset performance in under two minutes for the smallest dataset sizes.
- Bayesian models trained even faster, making them a competitive alternative when computational constraints are a priority.

---

#### Key Takeaways

- **Feasibility**: Low-data adaptation is viable for rhythmically homogeneous genres like samba and candombe, offering near-optimal performance with modest annotation efforts.
- **Optimal Strategy**: Fine-tuning pretrained models with data augmentation is the most effective approach, balancing performance and resource efficiency.
- **Implications**: This method opens the door to adapting beat tracking models for other underrepresented music traditions, reducing the barrier to entry for culturally diverse MIR applications.  

This exploration highlights the potential of data-efficient methods to expand the reach of MIR tools while respecting the uniqueness of diverse musical cultures.
