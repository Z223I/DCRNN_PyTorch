# Using SambaNova

## Running Original Code

```bash
python dcrnn_train_pytorch.py --config_filename=data/model/dcrnn_la.yaml
```

## Repo

```bash
git clone https://github.com/chnsh/DCRNN_PyTorch
```

## SSH to SambaNova

```bash
<your local machine> $ ssh <ANL username>@homes.cels.anl.gov
username@homes-01:~$ ssh sm-01.cels.anl.gov
username@sm-01.cels.anl.gov's password:
```

## Setup Environment

```bash
username@sm-01:~$ export PATH=$PATH:/opt/sambaflow/bin;export OMP_NUM_THREADS=1;source /opt/sambaflow/venv/bin/activate
```

## Cloning Repo on SambaNova

```bash
username@sm-01:~$ git clone https://github.com/chnsh/DCRNN_PyTorch
Cloning into 'DCRNN_PyTorch'...
Username for 'https://github.com': < username >
Password for 'https://username@github.com': < password >

## Git

Do any necessary git commands.

```bash
[username@medulla1 ~]$ cd DCRNN_PyTorch
[username@medulla1 DCRNN_PyTorch]$ git checkout < branch >
```

## Change Directory

```bash
# [username@medulla1 ~DCRNN_PyTorch]$ cd model/pytorch
or
[username@medulla1 ~]$ cd 3D-PyTorch/model/pytorch
```

## Commands Arguments

See the folling link for a list of arguments.
[https://confluence.cels.anl.gov/display/AI/SambaNova#SambaNova-Arguments](https://confluence.cels.anl.gov/display/AI/SambaNova#SambaNova-Arguments)

## Commands

```bash
python sn_boilerplate.py compile -b=1 --pef-name="sn_boilerplate" --output-folder="pef"
python sn_boilerplate.py test --pef="pef/sn_boilerplate/sn_boilerplate.pef"
python sn_boilerplate.py run --pef="pef/sn_boilerplate/sn_boilerplate.pef"
python sn_boilerplate.py measure-performance --pef="pef/sn_boilerplate/sn_boilerplate.pef"
```
