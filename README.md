# Probing Semantic Geometry in Word Embeddings

This project looks at how semantic meaning shows up in embedding space, using pretrained GloVe vectors rather than training a model from scratch.

The goal is to see how words are organized geometrically: whether similar concepts cluster together, whether categories can be recovered with clustering, and whether relationships (like gender) appear as directions.

## What I did

- visualized embeddings with PCA and t-SNE
- applied KMeans to test whether categories are recoverable
- evaluated clustering with silhouette score and adjusted Rand index
- tested analogies like king − man + woman ≈ queen
- projected words onto a gender direction to examine linear structure and bias

## What I found

The structure is present, though not cleanly separated.

Concrete categories such as animals and transport cluster more tightly, while abstract ones like emotions are more dispersed. Some relationships are approximately linear, though they sit within overlapping structure rather than distinct axes.

The gender direction example also highlights that embeddings reflect statistical patterns from the data, including bias.

## File

- `semantic_geometry.ipynb` — main notebook

## Takeaway

Semantic meaning is partially encoded in embedding geometry, though it remains distributed and entangled rather than neatly organized.
