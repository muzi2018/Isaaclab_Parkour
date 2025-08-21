## How to install 

```
cd IsaacLab ## going to IsaacLab
```

```
git clone https://github.com/cailab-hy/parkour_workspace.git ## cloning this repo
```

```
cd parkour_workspace && pip3 install -e .
```

```
cd parkour_tasks && pip3 install -e .
```

## How to train policies

### 1.1. Training Teacher Policy

```
python scripts/rsl_rl/train.py --task Isaac-Extreme-Parkour-Teacher-Unitree-Go2-v0 --seed 1 --headless
```

### 1.2. Training Student Policy

```
python scripts/rsl_rl/train.py --task Isaac-Extreme-Parkour-Student-Unitree-Go2-v0 --seed 1 --headless
```

## How to play your policy 

### 2.1. Pretrained Teacher Policy 

Download Teacher Policy by this [link](https://drive.google.com/file/d/1JtGzwkBixDHUWD_npz2Codc82tsaec_w/view?usp=sharing)

### 2.2. Playing Teacher Policy 

```
python scripts/rsl_rl/play.py --task Isaac-Extreme-Parkour-Teacher-Unitree-Go2-Play-v0 --num_envs 16
```

### 3.1 Pretrained Student Policy 

Download Student Policy by this [link]()

### 3.2. Playing Student Policy 

```
python scripts/rsl_rl/play.py --task Isaac-Extreme-Parkour-Student-Unitree-Go2-Play-v0 --num_envs 16
```

## How to play deploy in IsaacLab


### 3.1. Playing Teacher Policy 

```
python scripts/rsl_rl/demo.py --task Isaac-Extreme-Parkour-Teacher-Unitree-Go2-Play-v0 
```

### 3.2. Playing Student Policy 

```
python scripts/rsl_rl/demo.py --task Isaac-Extreme-Parkour-Student-Unitree-Go2-Play-v0 
```

## Testing your modules

```
cd parkour_test/ ## You can test your modules in here
```

## Visualize Control (ParkourViewportCameraController)

```
press 1 or 2: Going to environment

press 8: camera forward    

press 4: camera leftward   

press 6: camera rightward   

press 5: camera backward

press 0: Use free camera (can use mouse)

press 1: Not use free camera (default)
```

### Supported Parkour tasks

[o] [Extreme-Parkour](https://github.com/chengxuxin/extreme-parkour) 
