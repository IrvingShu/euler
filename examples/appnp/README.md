Predict then Propagate: Graph Neural Networks meet Personalized PageRank (APPNP)
============

Paper link: [Predict then Propagate: Graph Neural Networks meet Personalized PageRank](https://arxiv.org/abs/1810.05997)

Run
-------
```python
python run_appnp.py [--optional_params=params]
```

Params:

| Parameter Name | Default | Note |
| ----------------- | -------------- | ------------------------------- |
| dataset           | cora           | cora/pubmed/citeseer/ppi/reddit |
| hidden_dim        | 32             | hidden dimension                |
| layers            | 10             | GCN layer number                |
| batch_size        | 32            | running batch size              |
| num_epochs        | 20            | epochs to run                   |
| log_steps         | 20             | log per steps                   |
| model_dir         | ckpt           | checkpoint dir                  |
| learning_rate     | 0.01           | run learning rate               |
| optimizer         | adam           | run optimizer algorithm         |
| run_mode          | train          | train/evaluate                  |

Result
------
| Dataset | F1 |
| ---------- | ------------------ |
| cora       | 0.813              |
| pubmed     | 0.870              |
| citeseer   | 0.723              |

