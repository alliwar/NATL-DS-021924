# Recommendation Systems

The goal here is to introduce students to the varieties of recommendation systems: model-based vs. memory-based, content-based vs. collaborative-filtering.

## Learning Goals

- Describe the difference between content-based and collaborative-filtering algorithms
- Explain and use the cosine similarity metric
- Describe the algorithm of alternating least-squares
- Use the `surprise` package to build recommendation engines

## Lesson Materials

Two notebooks:
- [Jupyter Notebooks: Recommender Systems (without surprise)](recommender_systems.ipynb)
- [Jupyter Notebooks: Surprise](surprise.ipynb)

## Lesson Plan

### Introduction (5 Mins)

Intro hook is easy here since all students will be familiar with Netflix or Amazon recommendations!

### Content-Based Vs. Collaborative-Filtering & Memory-Based Vs. Model-Based (10 Mins)

Describe the different ideas here.

### Cosine Similarity (5 Mins)

Idea of representing comparanda as vectors. Remind students that vectors can live in a high-dimensional space, and it it still meaningful to speak of the plane that they define, and hence of the angle between them!

### Concept of Matrix Factorization and Latent Features (15 Mins)

Here I like to describe the factorization in terms of matrix dimensions: The full ratings (product) matrix will have a huge number of rows and columns, but if we factor it into the product of a users matrix and an items matrix, the inner dimensions (i.e. the number of columns in the user matrix and the number of rows in the items matrix) will be up to us. And in particular we can choose a relatively small number, which will represent these latent features (and we can choose the most predictive ones if we organize, say, singular vectors by their corresponding singular values etc.).

### Illustration of ALS in Code (10 Mins)

This is in some sense a poor approximation since we're filling unknowns with 0's, but they can still see the error of the model go down in successive iterations.

### Conclusion (5 Mins)

Conclude with relevance of matrix factorization techniques (like PCA and SVD) to rec systems.

### (Time Permitting) Surprise Notebook

Quick run-through of how to use the `surprise` library.

## Tips

### Greg Damico, 03/16/21

I like to use the whiteboard to draw the shapes of the matrices for matrix factorization à la ALS: Users x Items = Ratings. Then you can point out how the number of columns of the Users matrix (= number of columns of the Items matrix) can be any number we want, which should suggest to them the strategies of SVD and PCA. 
