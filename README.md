# XAI606
Project page for XAI606
https://youtu.be/mXw5vwnCJ20

# Dataset
`dataset/FINGER.json` contains train, val, test, OOD test dataset.

We actuated tendon-driven soft robot in real robot, and obtained paried data of (actuation, position).
Using this data, we aim to solve model identification to control soft robot.

## Train 
Training configs can be found in `code/configs` and, use arguments to choose model and dataset.


```
python3 code/main.py --configs "${MODEL}/${DATASET}.py"
```
Choose, 
`${MODEL}` from `[FC_PRIMNET, PRIMNET, PRIMNET_FULL]`
`${DATASET}` from `[FINGER, ABAQUS_32, ELASTICA]`
(e.g. To train `PureNN` on `FINGER` dataset,  `python3 code/main.py --configs "PRIMNET/FINGER.py"`)

# Contact
taerimyoon@korea.ac.kr
