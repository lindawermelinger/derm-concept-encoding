# A Systematic Comparison of Pretrained Visual Representations for Dermatologic Concept Encoding

**Linda Wermelinger, Simone Lionetti, Nipun Ranasekara, Marc Pouly, Alexander A. Navarini**

---

### [Paper (PDF)](./paper.pdf) &nbsp;&nbsp; [Poster (PDF)](./poster.pdf)

---

## Abstract
AI-based decision support systems have limited value for clinicians when they produce predictions without providing interpretable explanations. In dermatology, it is established that deep visual representations can encode clinically meaningful concepts, yet the consistency of this encoding across different model architectures and the degree of entanglement with dataset-specific characteristics remain under-explored. In this work, we present a systematic comparison of visual representations learned by 11 pretrained models, including general-purpose (ViT-B/16), self-supervised (DINOv2/v3), and multimodal architectures (CLIP, SigLIP), as well as those adapted specifically for the dermatological domain (e.g., MedSigLIP, MAKE). Using the SkinCon dataset, we evaluate image embeddings through dimensionality reduction, linear probing for concept-level classification, and distance-based evaluation. While several models achieve strong concept classification performance (MedSigLIP peak AUC-ROC: 0.9266 ± 0.0001), low-dimensional projections often show pronounced grouping by image source rather than dermatological concepts. Our analysis reveals that this clustering can be driven by specific non-clinical artifacts, such as the presence of a measurement ruler, which may overshadow clinical morphology in the representation space. Cross-dataset evaluation on the PH2 dataset indicates that while some visual attributes generalize (e.g., Black AUC-ROC: 0.861), others remain sensitive to differences in image modality and class imbalance. These findings provide a systematic overview of current model capabilities and illustrate the extent to which clinical semantics can remain entangled with dataset-specific features, highlighting an important area for refinement in the development of transparent AI-assisted dermatologic diagnosis.