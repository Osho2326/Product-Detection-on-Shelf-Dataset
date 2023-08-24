### Product-Detection-on-Shelf-Dataset

**Overview:**

FMCG(Fast-Moving Consumer Goods) brands require insights into retail shelves to help them improve their sales. One such insight comes from determining how many products of their brands’ are present versus how many products of competing brands are present on a retail store shelf. This requires finding the total number of products present on every shelf in a retail store.

**Problem Statement:** 

Given a grocery store shelf image, detect all products present in
the shelf image (detection only at product or no-product level).
The assignment requires you to implement a single-shot object
detector with only “one” anchor box per feature-map cell.
(MUST).

**Dataset:** 

- The dataset to be used for training/testing is the Grocery dataset.
Link to the dataset: (https://github.com/gulvarol/grocerydataset)
- Please use the following link to download ShelfImages.tar.gz
(contains train and test splits) and replace
GroceryDataset_part1/ShelfImages with this.
https://storage.googleapis.com/open_source_datasets/ShelfImage
S.tar.gz

**Insights in the problem statement:**

- The provided dataset is converted to TFRecords for easy compatibility with the TFOD API.
- Detection network used: SSD MobileDet.
- Precision reported is 0.78 and recall reported is 0.833.
- mAP reported was 0.78.
- A threshold of 0.6 was used in order to obtain the number of products per test image.
