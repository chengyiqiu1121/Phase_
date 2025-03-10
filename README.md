# Phase_

The official code repo of the paper "Phojan: Phase-based, Invisible Backdoor Attack"

# Ho To Use?

## Train

You need to clone the code to your own device, and cd to the `run` folder, then run:

```she
python train.py dataset_name=cifar10 model=resnet18 attack=phase
```

or other attack:

```shell
python train.py dataset_name=cifar10 model=resnet18 attack=ftrojan
```

When training, a result folder will be made and named as `/home/chengyiqiu/code/INBA/results/cifar10/phase/resnet18/20241210213438`. The `.pth` file and other files will be lying there.

 ## Test

After training (or download the checkpoints we provided), you can cd the `run` folder and run this command to evalate the BA, ASR:

```shell
python eval_acc.py --path /home/chengyiqiu/code/INBA/results/cifar10/phase/resnet18/20241210190231
```

and this command to evaluate the SSIM, PSNR, LPIPS:

```shell
python eval_ssim.py --path /home/chengyiqiu/code/INBA/results/imagenette/phase/resnet18/20241220131213
```

just need to replace the target folder to your own path.

# Checkpoint

## CIFAR10-ResNet18
| Name   | Link                                                         | Passport |
| ------ | ------------------------------------------------------------ | -------- |
| Phojan | [Baidu Driver](https://pan.baidu.com/s/1VnHQdKn9ANXkohf66HDntA) | `wue3`   |
| DUBA   | [Baidu Driver](https://pan.baidu.com/s/19igEsHyVS8sCNzOklmcIsA) | `sqh1`   |
| FIBA   | [Baidu Driver](https://pan.baidu.com/s/1tkwBTRDv8AtkZVjCnF32Iw) | `drb3`   |
| CTRL   | [Baidu Driver](https://pan.baidu.com/s/1nutIRQ7M0poqZ4zDvmLAiQ) | `behb`   |
| ...    | ...                                                          | ...      |

More checkpoints will be uploaded in the future.

# ToDo

- Release code: Yes.
- Upload Checkpoint: Yes.
- Tiny code: No.
- Add citation: No.