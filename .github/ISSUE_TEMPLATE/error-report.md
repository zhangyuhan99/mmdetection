---
name: 
about: Create a report to help us improve
title: ''
labels: ''
assignees: ''

---

Thanks for your error report and we appreciate it a lot.

**Checklist**

1. I have searched related issues but cannot get the expected help.
2. I have read the [FAQ documentation](https://mmdetection.readthedocs.io/en/latest/faq.html) but cannot get the expected help.
3. The bug has not been fixed in the latest version.

**Describe the bug**
A clear and concise description of what the bug is.
Can't verify demo，and after training the dataset, the test job cannot be completed.During the training process, there was userwarning.

**Reproduction**

1. What command or script did you run?
python demo/image_demo.py demo/demo.jpg configs\rotated_faster_rcnn\rotated_faster_rcnn_r50_fpn_1x_dota_le90.py weights/rotated_faster_rcnn_r50_fpn_1x_dota_le90-0393aa5c.pth demo/vis.jpg

2. Did you make any modifications on the code or config? Did you understand what you have modified
 no yes
4. What dataset did you use?
 dota
**Environment**
linux torch==1.9.0+cu111 torch==0.10.0+cu111 mmdet==2.22.0 mmcv-full==1.4.5 mmrotate==0.1.0
1. Please run `python mmdet/utils/collect_env.py` to collect necessary environment information and paste it here.
2. You may add addition that may be helpful for locating the problem, such as
    - How you installed PyTorch [e.g., pip, conda, source]
    - Other environment variables that may be related (such as `$PATH`, `$LD_LIBRARY_PATH`, `$PYTHONPATH`, etc.)

**Error traceback**
If applicable, paste the error trackback here.

```none
UserWarning: DeprecationWarning: `num_anchors` is deprecated, for consistency or also use `num_base_priors` instead
  warnings.warn('DeprecationWarning: `num_anchors` is deprecated, '
home/lab208/anaconda3/envs/openmmlab/lib/python3.7/site-packages/mmdet/models/dense_heads/anchor_head.py:123: UserWarning: DeprecationWarning: anchor_generator is deprecated, please use "prior_generator" instead
```

**Bug fix**
If you have already identified the reason, you can provide the information here. If you are willing to create a PR to fix it, please also leave a comment here and that would be much appreciated!
