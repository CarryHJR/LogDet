## LogDetMini 实验

|         方案         |  mAP  | Training time/h |
| :------------------: | :---: | :-------------: |
|         r101         | 0.344 |       0.4       |
|       r101_3x        | 0.447 |        \        |
|     r101_3x_flip     | 0.455 |        \        |
| r101_3x_flip_softnms | 0.457 |        \        |
|       r101_12x       | 0.452 |       1.5       |
|       swint_3x       | 0.454 |       0.6       |
|       bigsize       | 0.478 |       0.53       |
|       bigsize+autoaug       | 0.497 |       \       |
|       bigsize+autoaug+dcn       | 0.509 |       \       |
|       bigsize+autoaug+dcn+anchor       | 0.516 |       \       |
| swinb_3x_800-1400_anchor_bs2x8 | 0.507| 0.97 | 
| swinb_3x_800-1400_anchor_bs2x8_db| 0.553| 1.6 | 
| convb_3x_bs2x8_1k| 0.46 | \ |
|convb_3x_bs2x8_1k_800-1400 | 0.534 | 1.4|
|swinb_3x | 0.466 | 0.87|
| swinb_3x_800-1400 | 0.539 | \ |

