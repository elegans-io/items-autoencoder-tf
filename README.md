# Encoder NN for items to items

The program calculates the vector representation from items 

## Usage:

### Help

```bash
(tensorflow) $ ./itemsEncoder.py --help
usage: itemsEncoder.py [-h] [--input-folder INPUT_FOLDER]
                       [--out-folder OUT_FOLDER] [--batch-size BATCH_SIZE]
                       [--embedding-size EMBEDDING_SIZE]
                       [--num-neg-sampled NUM_NEG_SAMPLED] [--epochs EPOCHS]
                       [--learning-rate LEARNING_RATE]

Train an encoder NN to extract a vector representation from items create a
final_embeddings_<embedding_size>.tsv file inside the output folder

optional arguments:
  -h, --help            show this help message and exit
  --input-folder INPUT_FOLDER
                        input data directory with COOCCURRENCE_* folder
  --out-folder OUT_FOLDER
                        The log directory for TensorBoard summaries.
  --batch-size BATCH_SIZE
                        the batch size
  --embedding-size EMBEDDING_SIZE
                        the embedding size
  --num-neg-sampled NUM_NEG_SAMPLED
                        the number of negative sampled items
  --epochs EPOCHS       the number of training epochs
  --learning-rate LEARNING_RATE
                        the learning rate
```

### Run

```bash
./itemsEncoder.py --input-folder ../orac-sdk/ETL_FOLDER
```

