# Time-Series Representation Learning via Temporal and Contextual Contrasting (TS-TCC) [[Paper](https://www.ijcai.org/proceedings/2021/0324.pdf)] [[Cite](#citation)]
#### *by: Emadeldeen Eldele, Mohamed Ragab, Zhenghua Chen, Min Wu, Chee Keong Kwoh, Xiaoli Li, and Cuntai Guan*
#### This work is accepted for publication in the International Joint Conferences on Artificial Intelligence (IJCAI-21) (Acceptance Rate: 13.9%).

## Updates
1. We extended our method to semi-supervised settings (CA-TCC). Check the manuscript [Self-supervised Contrastive Representation Learning for Semi-supervised Time-Series Classification](http://arxiv.org/abs/2208.06616) for more details. The [code is available here](https://github.com/emadeldeen24/CA-TCC).
2. **CA-TCC** is now accepted in the IEEE Transactions on Pattern Analysis and Machine Intelligence (**TPAMI**).

---

## Abstract
<p align="center">
<img src="misc/TS_TCC.png" width="400">
</p>

This work proposes an unsupervised **T**ime-**S**eries representation learning framework via **T**emporal and **C**ontextual **C**ontrasting (**TS-TCC**) to learn from unlabeled time-series data. Key contributions include:
- Temporal contrasting for robust temporal representations.
- Contextual contrasting for discriminative representations.

Experiments demonstrate state-of-the-art performance on real-world datasets and effectiveness in few-labeled and transfer learning scenarios.

---

## Requirements

### Python Environment
- Python 3.x
- Install dependencies via `requirements.txt`:
  ```bash
  pip install -r requirements.txt
  ```

### CUDA and PyTorch
- Install PyTorch and CUDA support:
  ```bash
  conda install pytorch==1.7.0 torchvision==0.8.0 torchaudio==0.7.0 cudatoolkit=11.0 -c pytorch
  ```
### Running the Pipeline

For Linux:
```bash
./ca_tcc_pipelin.sh
```

For windows:
```bash
run.bat
```

## Datasets
### Download Links
- [Sleep-EDF](https://gist.github.com/emadeldeen24/a22691e36759934e53984289a94cb09b)
- [HAR](https://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones)
- [Epilepsy](https://archive.ics.uci.edu/ml/datasets/Epileptic+Seizure+Recognition)  
- [Fault Diagnosis](https://mb.uni-paderborn.de/en/kat/main-research/datacenter/bearing-datacenter/data-sets-and-download)

---

## Training Instructions

### Modes
- **Random Initialization**
- **Supervised training**
- **Self-supervised training**
- **Fine-tuning**
- **Training a linear classifier**

### Example Command
```bash
python main.py --experiment_description exp1 --run_description run_1 --seed 123 --training_mode self_supervised --selected_dataset HAR
```

---

## Results
- Experiment logs and classification reports are stored in the `experiments_logs` folder by default.

---

## Citation
Please cite this work if it is useful to your research:
```bibtex
@inproceedings{ijcai2021-324,
  title     = {Time-Series Representation Learning via Temporal and Contextual Contrasting},
  author    = {Eldele, Emadeldeen et al.},
  booktitle = {Proceedings of IJCAI-21},
  pages     = {2352--2359},
  year      = {2021},
}
```

```bibtex
@article{emadeldeen2022catcc,
  title   = {Self-supervised Contrastive Representation Learning for Semi-supervised Time-Series Classification},
  author  = {Eldele, Emadeldeen et al.},
  journal = {arXiv preprint arXiv:2208.06616},
  year    = {2022}
}
```

---

## Contact
For any issues/questions, contact Emadeldeen Eldele (email: emad0002{at}e.ntu.edu.sg).

---
