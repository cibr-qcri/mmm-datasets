# mmm-datasets

Public datasets from our [paper](https://arxiv.org/abs/1910.12244) on investigating MMM Ponzi scheme on Bitcoin.

The following datasets are *non-filtered* crawls of BitcoinTalk user pofiles and BlockchainInfo public tags from 2019. Each dataset is a JSON file (i.e., lines of JSON strings) that is compressed using ZIP archive file format. Make sure to uncompress the file before parsing it. Make sure to follow the filtering described in the paper to get MMM-specific users and tags.

## [users.json.zip](https://raw.githubusercontent.com/cibr-qcri/mmm-datasets/main/users.json.zip)

This dataset contains public BitcoinTalk profile info of 40,971 users grouped by their Bitcoin addresses (a total of 39,321 unique addresses). Each line in the dataset file is a JSON dump of a key/value object describing the linked users of a unique Bitcoin address, as follows:

| Key     | Value                                                                                         |
|---------|-----------------------------------------------------------------------------------------------|
| address | Bitcoin address                                                                               |
| users   | A list of user data, each consisting of the user's public profile info (name, location, etc.) |

## [tags.json.zip](https://raw.githubusercontent.com/cibr-qcri/mmm-datasets/main/tags.json.zip)

This dataset contains 30,012 public BlockchainInfo tags of unique Bitcoin addresses. Each line in the dataset file is a JSON dump of a key/value object describing a tag of a Bitcoin address, as follows:

| Key     | Value                                                  |
|---------|--------------------------------------------------------|
| address | Bitcoin address                                        |
| tag     | Tag data consisting of its value and verification info |

## Citation

If you use Dizzy or any of its datasets, please cite the following [publication](https://arxiv.org/abs/1910.12244):
```
@inproceedings{boshmaf2020investigating,
  title={Investigating MMM Ponzi scheme on bitcoin},
  author={Boshmaf, Yazan and Elvitigala, Charitha and Al Jawaheri, Husam and Wijesekera, Primal and Al Sabah, Mashael},
  booktitle={Proceedings of the 15th ACM Asia Conference on Computer and Communications Security},
  pages={519--530},
  year={2020}
}
```
