# base5yy
Detecting Repeated Interactions with One Contract
from collections import Counter

targets = Counter(tx["to"] for tx in block.transactions if tx["to"])
print(targets.most_common(3))
