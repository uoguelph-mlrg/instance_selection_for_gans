## Change Log
This log documents the changes made to the original BigGAN-PyTorch repo.

1. Added instance selection to get_data_loaders function in utils.py (L588-L603). Also add corresponding args (L37-L48).
2. Added calculate_image_manifold.py for preprocessing and saving feature embeddings of real images. To be used for calculating Precision, Recall, Density, and Coverage (PRDC) metrics.
3. Added PRDC evaluation code to inception_utils.py (L271-L357, L371, L382). Code from https://github.com/clovaai/generative-evaluation-prdc.
4. Added PRDC to logging in train_fns.py. (L168, L185-L186).
5. Added option to stop training based on number of iterations. (L175-L177 in train.py, and L206-L207 in utils.py).
