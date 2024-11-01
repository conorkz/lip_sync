# Audio-based Lip Synchronization
This lip-sync system based on python disentangles the objective into three sequential tasks:

(1) face video generation with a canonical expression

(2) audio-driven lip-sync and

(3) face enhancement for improving photo-realism.
### Environment
```
git clone https://github.com/vinthony/lip_sync.git
cd lip_sync
conda create -n lip_sync python=3.8
conda activate lip_sync

conda install ffmpeg

# Please follow the instructions from https://pytorch.org/get-started/previous-versions/
# This installation command only works on CUDA 11.1
pip install torch==1.9.0+cu111 torchvision==0.10.0+cu111 -f https://download.pytorch.org/whl/torch_stable.html

pip install   
 -r requirements.txt
```
### Inference
```
python3 inference.py \
  --face examples/face/1.mp4 \
  --audio examples/audio/1.wav \
  --outfile results/1_1.mp4
```
