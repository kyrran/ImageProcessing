# SimCLR Coursework: Exploring Contrastive Learning and Transfer Learning

In this coursework, I explored the popular self-supervised contrastive learning approach, SimCLR. The goal was to implement key components of SimCLR, including a suitable data augmentation strategy for generating positive pairs, the SimCLR loss function, and the SimCLR training step. Additionally, I applied transfer learning strategies to evaluate the performance of different pre-trained models on a downstream classification task.

## Coursework Structure

The coursework is divided into three parts:

- **Part A**: Implementation of a suitable dataset for contrastive model training;
- **Part B**: Implementation of the SimCLR loss and training step;
- **Part C**: Implementation of transfer learning strategies (linear probing and fine-tuning) for model evaluation.

## Key Achievements

- Designed and implemented a custom **contrastive dataset** using advanced data augmentation techniques.
- Developed the **SimCLR loss function** following the original framework, which effectively trains the model to pull together positive pairs and push apart negative pairs.
- Successfully implemented the **SimCLR training step** using PyTorch Lightning, which ensured scalability and efficient experimentation.
- Applied **transfer learning** strategies, including **linear probing** and **fine-tuning**, to assess how well the learned representations perform on downstream tasks.

## Results & Analysis

### Performance Metrics

- **Contrastive Learning**: SimCLR model improved feature representation learning by utilizing strong augmentations and contrastive loss.
- **Transfer Learning**: Linear probing and fine-tuning on the downstream classification task showed that fine-tuning outperformed linear probing when deeper layers of the model were involved.

### Data Augmentation and Contrastive Loss

- Augmentation techniques, such as **random cropping**, **color jitter**, and **Gaussian blur**, were crucial for generating positive pairs that helped the model learn invariant features.
- The **SimCLR loss function** effectively distinguished between positive and negative pairs using the temperature parameter to scale similarities.

### Transfer Learning Analysis

- **Linear Probing**: Fine-tuned the top layer of the model, yielding decent results on the downstream task but limited compared to full model fine-tuning.
- **Fine-Tuning**: Full model fine-tuning significantly improved the classification accuracy, especially when using the representations learned via contrastive learning in SimCLR.

## Technical Implementation

### Part A: Contrastive Dataset

A carefully crafted dataset that leverages data augmentation techniques to create positive and negative pairs for training the contrastive model.

### Part B: SimCLR Loss and Training Step

Implemented the SimCLR loss function, which calculates similarity between embeddings, and designed a training loop in PyTorch Lightning for contrastive learning.

### Part C: Transfer Learning

Implemented two main strategies for transfer learning:
1. **Linear Probing**: Training only the final classifier layer while keeping the learned representations frozen.
2. **Fine-Tuning**: Training the entire model, including all layers, to adapt the learned features to a new task.

## Conclusion

Through this coursework, I gained hands-on experience in implementing a self-supervised learning model and applying transfer learning strategies. The SimCLR model showed the importance of contrastive learning in feature extraction, and transfer learning strategies demonstrated the adaptability of these learned features to new tasks.

This project highlights my skills in:
- **Self-supervised learning** using contrastive loss techniques.
- **Transfer learning** methods for adapting pre-trained models.
- Proficiency in **PyTorch** and **PyTorch Lightning** for scalable machine learning workflows.
