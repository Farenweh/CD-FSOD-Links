# 航空遥感跨域少样本目标检测资源汇总

本页面提供论文《航空遥感场景跨域少样本目标检测进展研究》中涉及的数据集与代表性模型整理快速访问。

说明：
- “/”表示未公开 arXiv 页面或官方 GitHub/项目页面。
- 部分项目未提供 GitHub 仓库，但提供项目主页；此类链接暂列入“GitHub/项目页面”。
- 链接核对日期：2026-05-27。

## 数据集

| 数据集 | 在本文中的用途/说明 | arXiv/论文页面 | GitHub/项目页面 |
|---|---|---|---|
| COCO | 通用目标检测/实例分割数据集；论文中作为通用源域与性能对比数据集出现 | [arXiv](https://arxiv.org/abs/1405.0312) | [GitHub/项目页](https://github.com/cocodataset/cocoapi) |
| LVIS | 大词汇实例分割数据集；论文中用于开放词汇/大模型检测性能讨论 | [arXiv](https://arxiv.org/abs/1908.03195) | [GitHub/项目页](https://github.com/lvis-dataset/lvis-api) |
| MoFSOD | 多领域少样本目标检测基准 | [arXiv](https://arxiv.org/abs/2207.11169) | [GitHub/项目页](https://github.com/amazon-research/few-shot-object-detection-benchmark) |
| CD-FSOD (Xiong) | 跨域少样本目标检测基准；本文重点情境之一 | [arXiv](https://arxiv.org/abs/2210.05311) | [GitHub/项目页](https://github.com/woody-panda/CD-FSOD) |
| CD-FSOD (Fu) | 跨域少样本目标检测基准（ECCV 2024，Fu Yuqian） | [arXiv](https://arxiv.org/abs/2402.03094) | [GitHub/项目页](https://github.com/lovelyqian/CDFSOD-benchmark) |
| DIOR | 光学遥感目标检测数据集；本文 COCO→DIOR 设置的目标域 | [arXiv](https://arxiv.org/abs/1909.00133) | [官方数据集页](https://gcheng-nwpu.github.io/) |
| DOTA | 航空遥感旋转目标检测数据集 | [arXiv](https://arxiv.org/abs/1711.10398) | [GitHub/项目页](https://github.com/CAPTAIN-WHU/DOTA_devkit) |
| xView | 大规模俯视遥感目标检测数据集 | [arXiv](https://arxiv.org/abs/1802.07856) | [GitHub/项目页](https://github.com/DIUx-xView/xView1_baseline) |
| VEDAI | 航空图像车辆检测小目标基准 | / | [官方数据集页](https://downloads.greyc.fr/vedai/) |
| NWPU VHR-10 | 高分辨率遥感目标检测数据集 | [论文页](https://www.sciencedirect.com/science/article/pii/S0924271614002119) | [官方数据集页](https://gcheng-nwpu.github.io/) |

## 模型与算法

| 模型/算法 | 方法类别/说明 | arXiv/论文页面 | GitHub/项目页面 |
|---|---|---|---|
| Faster R-CNN | 基础两阶段检测框架 | [arXiv](https://arxiv.org/abs/1506.01497) | [GitHub/项目页](https://github.com/rbgirshick/py-faster-rcnn) |
| DA Faster R-CNN | 迁移/域对齐 | [arXiv](https://arxiv.org/abs/1803.03243) | [GitHub/项目页](https://github.com/yuhuayc/da-faster-rcnn) |
| SWDA | 迁移/域对齐 | [arXiv](https://arxiv.org/abs/1812.04798) | [GitHub/项目页](https://github.com/VisionLearningGroup/DA_Detection) |
| SAPNet | 迁移/域对齐 | [arXiv](https://arxiv.org/abs/2003.12979) | [GitLab/项目页](https://isrc.iscas.ac.cn/gitlab/research/domain-adaption) |
| Adaptive Teacher | 迁移/域对齐；教师-学生框架 | [arXiv](https://arxiv.org/abs/2111.13216) | [GitHub/项目页](https://github.com/facebookresearch/adaptive_teacher) |
| Meta R-CNN | 元学习/少样本检测 | [arXiv](https://arxiv.org/abs/1909.13032) | / |
| Attention-RPN / Multi-Relation Detector | 元学习/少样本检测 | [arXiv](https://arxiv.org/abs/1908.01998) | [GitHub/项目页](https://github.com/fanq15/Few-Shot-Object-Detection-Dataset) |
| TFA / TFA w/cos | 少样本微调基线 | [arXiv](https://arxiv.org/abs/2003.06957) | [GitHub/项目页](https://github.com/ucbdrive/few-shot-object-detection) |
| FSCE | 度量学习/对比候选区域编码 | [arXiv](https://arxiv.org/abs/2103.05950) | [GitHub/项目页](https://github.com/megvii-research/FSCE) |
| DeFRCN | 少样本检测；解耦 Faster R-CNN | [arXiv](https://arxiv.org/abs/2108.09017) | [GitHub/项目页](https://github.com/er-muyue/DeFRCN) |
| Distill-CDFSOD | 跨域少样本检测蒸馏基线；CD-FSOD 论文中的强基线 | [arXiv](https://arxiv.org/abs/2210.05311) | [GitHub/项目页](https://github.com/woody-panda/CD-FSOD) |
| ViTDet / ViTDeT-FT | ViT 检测骨干/微调基线 | [arXiv](https://arxiv.org/abs/2203.16527) | [GitHub/项目页](https://github.com/facebookresearch/detectron2/tree/main/projects/ViTDet) |
| Detic / Detic-FT | 开放词汇/长尾目标检测 | [arXiv](https://arxiv.org/abs/2201.02605) | [GitHub/项目页](https://github.com/facebookresearch/Detic) |
| DE-ViT / DE-ViT-FT | 基于 ViT 的无需微调少样本检测 | [arXiv](https://arxiv.org/abs/2309.12969) | [GitHub/项目页](https://mlzxy.github.io/devit/) |
| CD-ViTO | 跨域少样本检测；增强开放集检测器 | [arXiv](https://arxiv.org/abs/2402.03094) | [GitHub/项目页](https://github.com/lovelyqian/CDFSOD-benchmark) |
| Meta-DETR | 图像级少样本 DETR 检测器 | [arXiv](https://arxiv.org/abs/2208.00219) | [GitHub/项目页](https://github.com/ZhangGongjie/Meta-DETR) |
| Hallucination FSOD | 生成式特征增强 | [arXiv](https://arxiv.org/abs/2105.01294) | / |
| Synthetic Data for FSOD | 文本生成图像/copy-paste 合成增强 | [arXiv](https://arxiv.org/abs/2303.13221) | / |
| MPAD | 多视角数据增强/扩散生成增强 | [arXiv](https://arxiv.org/abs/2502.18195) | [GitHub/项目页](https://github.com/nvakhoa/MPAD) |
| AeroGen | 遥感目标检测扩散生成增强 | [arXiv](https://arxiv.org/abs/2411.15497) | [GitHub/项目页](https://github.com/Sonettoo/AeroGen) |
| Control Copy-Paste | 遥感少样本检测可控扩散增强 | [arXiv](https://arxiv.org/abs/2507.21816) | / |
| Domain-RAG | 跨域少样本检测检索增强生成 | [arXiv](https://arxiv.org/abs/2506.05872) | [GitHub/项目页](https://github.com/LiYu0524/Domain-RAG) |
| CLIP | 视觉语言预训练基础模型 | [arXiv](https://arxiv.org/abs/2103.00020) | [GitHub/项目页](https://github.com/openai/CLIP) |
| RegionCLIP | 区域级视觉语言预训练 | [arXiv](https://arxiv.org/abs/2112.09106) | [GitHub/项目页](https://github.com/microsoft/RegionCLIP) |
| PromptDet | 开放词汇检测/提示学习 | [arXiv](https://arxiv.org/abs/2203.16513) | [GitHub/项目页](https://fcjian.github.io/promptdet/) |
| DINO | DETR 系列检测器；Grounding DINO 基础之一 | [arXiv](https://arxiv.org/abs/2203.03605) | [GitHub/项目页](https://github.com/IDEACVR/DINO) |
| DETR | Transformer 目标检测基础框架 | [arXiv](https://arxiv.org/abs/2005.12872) | [GitHub/项目页](https://github.com/facebookresearch/detr) |
| Grounding DINO | 开放集/视觉语言目标检测 | [arXiv](https://arxiv.org/abs/2303.05499) | [GitHub/项目页](https://github.com/IDEA-Research/GroundingDINO) |
| RT CD-MFSOD / Rich Text CDMM-FSOD | 基于丰富文本的跨域多模态少样本检测 | [arXiv](https://arxiv.org/abs/2403.16188) | / |
| LAE-DINO | 遥感开放词汇目标检测基础模型 | [arXiv](https://arxiv.org/abs/2408.09110) | / |
| ETS | 基于基础模型的增强-搜索跨域少样本检测策略 | [arXiv](https://arxiv.org/abs/2504.04517) | [GitHub/项目页](https://github.com/jaychempan/ETS) |
| Mixture of DETR and Vision Foundation Models | 检测器与视觉基础模型融合 | / | / |
| Rex-Omni | 多模态大模型目标检测/下一点预测 | [arXiv](https://arxiv.org/abs/2510.12798) | [GitHub/项目页](https://github.com/IDEA-Research/Rex-Omni) |
| StyleProto | 风格增强原型学习跨域少样本检测 | / | / |
