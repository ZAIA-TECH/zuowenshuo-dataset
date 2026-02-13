# 作文说AI作文批改公开数据集 (Zuowenshuo AI Essay Correction Dataset)

本数据集由[作文说](http://www.zuowenshuo.cn)提供，旨在支持人工智能在教育领域的学术研究与交流，特别是针对中文作文自动批改、人机协同评价及教学评一致性等方向的研究。

**声明：本数据集仅供学术研究与交流使用，严格禁止用于任何商业用途。**

## 数据集内容

本数据集包含三个主要部分，全部来自真实的教学场景（已脱敏）：

### 1. 01_作文图片数据集 (Essay Image Dataset)
包含学生手写作文的原始扫描/拍摄图片。

*   **注意**: 由于图片数据总量较大，已分割为多个压缩包 (`images_part1.zip`, `images_part2.zip`, ...)。
*   使用时请下载所有 `images_part*.zip` 文件并解压。

### 2. 02_作文批改数据集 (Essay Correction Dataset)
包含作文的文本内容、AI初评结果、教师复核后的最终评分与评语等详细数据。
*   *注：由于原始CSV文件较大，已压缩为 `作文批改数据集.csv.zip`，使用前请解压。*

**数据字段概览:**
*   **基础信息**: `id` (订单ID), `article_title` (标题), `article_content` (正文)
*   **任务信息**: `grade` (年级 1-12), `subject` (学科), `word_counts` (字数要求), `writing_type` (文体)
*   **批改结果**: `score` (总分), `score_detail` (维度得分), `summary` (总评), `report` (精批报告)

**统计概览:**
*   **总记录数**: 15,000篇 (分层抽样：小学40%，初中40%，高中20%)
*   **平均字数**: 590字

### 3. 03_人工复核数据集 (Human Review Dataset)
专注于教师对AI评价进行修改和干预的记录，用于研究人机协同行为。

## 使用条款与许可 (License & Terms of Use)

1.  **非商业用途 (Non-Commercial Use Only)**: 本数据集仅限用于非营利性的学术研究、教学和科学交流。任何个人或机构不得将本数据集的全部或部分用于商业产品、服务或任何形式的营利性活动。
2.  **引用说明 (Citation)**: 在学术论文或研究成果中使用本数据集时，请注明来源“作文说AI作文批改公开数据集”或引用相关论文。
    ```bibtex
    @dataset{zuowensuo_dataset_2026,
      title = {作文说数据集：面向"教学评一致"的教师-AI协同批改系统数据集},
      author = {Zaiatech},
      year = {2026},
      publisher = {GitHub},
      url = {https://github.com/ZAIA-TECH/zuowenshuo-dataset}
    }
    ```
3.  **免责声明**: 数据集提供方不对数据的使用后果承担任何责任。

## 联系我们 (Contact)

我们非常欢迎任何形式的学术交流与合作。如果您对数据集有任何疑问，或希望探讨基于此数据的研究合作，请联系我们：

*   **邮箱**: zayaTech@163.com
