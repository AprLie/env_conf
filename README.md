# env_conf

## tmux
```
ln -s -f .tmux/.tmux.conf  
cp .tmux/.tmux.conf.local .    
```

restart tmux server by  
```
tmux kill-server  
```

## conda
有时需要sudo,否则无法运行,注意目录放用户下  
```
bash xxx.sh
```
根据yaml创建  
```
conda env create -f xxx.yaml
```
有时在`conda activate env`会显示`CommandNotFoundError: Your shell has not been properly configured to use 'conda activate'.`  
解决:  
```
source ~/anaconda3/etc/profile.d/conda.sh
```
