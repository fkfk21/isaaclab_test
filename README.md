# isaaclab installation 

https://isaac-sim.github.io/IsaacLab/source/setup/installation/pip_installation.html


環境: ubuntu 22.04, CUDA 12.1

Prerequires
install poetry
```bash
poetry config virtualenvs.in-project true
```


```bash
poetry install --no-root
source (poetry env info --path)/bin/activate.fish # activate virtual environment
vcs import . < isaaclab.repos
isaaclab/isaaaclab.sh --install  # install packages iteratively through pip
```

## memo
### install version
pytorch 2.4.0 for cuda12.1
isaac sim <- followed isaaclab installation

isaaclab/isaaclab.sh install packages directly


## reinforcement learning

```bash
./isaaclab.sh -p source/standalone/workflows/rsl_rl/train.py --task Isaac-Velocity-Flat-Mevius-v0 --num_envs 1024 --max-iterations 20000
```
ログの保存先
`~/core_ws/isaaclab_test/isaaclab/logs/rsl_rl/mevius_flat`




## ToDo

- lab_assetsのmevius.py
  - mevius.usdの作成
    - 例: anymalにならうと  usd_path=f"{ISAACLAB_NUCLEUS_DIR}/Robots/Mevius/mevius.usd",
  - ANYDRIVE_3_SIMPLE_ACTUATOR_CFGに相当するactuatorモデルの設定
  - InitialStateCfgの修正。meviusに合わせる
  - meviusのセンサー設定 (realsense t265)






