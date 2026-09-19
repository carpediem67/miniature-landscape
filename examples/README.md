# 案例与提示词 · Examples & prompts

[English guide](../README.md) · [中文说明](../README.zh-CN.md)

## 如何使用 · How to use

这些是创作者选定的实际生成结果，不是地理精度标杆。选择一张适合目标的图片作为**风格参考**，并提供新的地点；只继承材质、镜头与景深，不复制原城市的形状或地标。图片数量、建筑密度和留白由用户要求决定。

These are creator-selected generation results, not cartographic accuracy benchmarks. Choose an image as a **style reference** and name a new place. Transfer its materials, camera and depth of field, while replacing the original city's shape and landmarks. The user's request determines image count, density and negative space.

| 地点 / Place | 原图 / Image | 实际提示词 / Actual prompt | 输入方式 / Input |
| --- | --- | --- | --- |
| 阿勒泰 / Altay | [PNG](images/altay.png) | [TXT](prompts/altay.txt) | 纽约风格参考 / New York reference |
| 旧金山 / San Francisco | [PNG](images/san-francisco.png) | [TXT](prompts/san-francisco.txt) | 纽约风格参考 / New York reference |
| 悉尼 / Sydney | [PNG](images/sydney.png) | [TXT](prompts/sydney.txt) | 纽约风格参考 / New York reference |
| 里约热内卢 / Rio de Janeiro | [PNG](images/rio-de-janeiro.png) | [TXT](prompts/rio-de-janeiro.txt) | 纽约风格参考 / New York reference |
| 上海 / Shanghai | [PNG](images/shanghai.png) | [TXT](prompts/shanghai.txt) | 纽约风格参考 / New York reference |
| 巴黎 / Paris | [PNG](images/paris.png) | [TXT](prompts/paris.txt) | 纽约风格参考 / New York reference |
| 伦敦 / London | [PNG](images/london.png) | [TXT](prompts/london.txt) | 纽约风格参考 / New York reference |
| 杭州 / Hangzhou | [PNG](images/hangzhou.png) | [TXT](prompts/hangzhou.txt) | 文字生成 / Text only |
| 深圳 / Shenzhen | [PNG](images/shenzhen.png) | [TXT](prompts/shenzhen.txt) | 文字生成 / Text only |

## 参考与复现 · Reference and reproduction

七张参考图生成案例使用了同一张[纽约风格图](reference/new-york.png)。该图是辅助输入，不计入上面的九张精选案例。杭州与深圳是本次明确选定的早期版本，使用各自原始提示词，没有替换成后来系列中同名城市的另一张图。

Seven examples used the same [New York style image](reference/new-york.png). It is a supporting input, separate from the nine gallery selections. Hangzhou and Shenzhen are the specifically selected earlier versions, paired with their own original prompts rather than later same-city alternatives.

提示词保留生成时的中文原文；英文用法见主说明。不同工具对“参考图”参数的定义不同，应按当前工具的接口传递图片，不照搬某个固定 API 字段。所有案例使用内置 image_gen，未声称绑定某个底层模型版本。结果具有随机性，不能保证按提示词逐像素复现。

The prompt files preserve the original Chinese text used for generation; the main English guide provides usage examples. Supply reference images according to the current tool's interface rather than assuming a fixed API field. All examples used built-in image_gen; no underlying model version is asserted. Outputs are stochastic and are not guaranteed to reproduce pixel for pixel.

图像未经裁切、重绘或压缩转换。尺寸、SHA-256 和输入方式记录在 [manifest.json](manifest.json)。阿勒泰表现地区景观；各地均有距离压缩、建筑简化及生成式细节，不适用于导航、测绘或建筑校核。

The images have not been cropped, repainted or transcoded. Dimensions, SHA-256 hashes and input types are recorded in [manifest.json](manifest.json). Altay represents a regional landscape. All scenes contain compressed distances, simplified architecture and generated details; they are not suitable for navigation, surveying or architectural verification.

## 许可 · License

案例、提示词和参考图随仓库按 [MIT](../LICENSE) 发布。全部图像为 AI 生成作品。

The examples, prompts and reference image are included under the repository's [MIT license](../LICENSE). All images are AI-generated.

