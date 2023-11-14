1. 配置MapTR环境，参考：https://github.com/hustvl/MapTR/blob/main/docs/install.md
2. 安装osmread包，参考：https://github.com/dezhin/osmread，在`./osmread`目录下`python setup.py install`
3. 安装剩余依赖：`pip install -r requirement.txt`
4. 运行：`python main.py`，其中可以在配置文件中更改配置。需要在`./MapTR-infer/projects/configs/maptr/maptr_lxl.py`中更改数据集路径，并参考 https://github.com/hustvl/MapTR/blob/main/docs/prepare_dataset.md 生成数据标注。
5. 生成的中间osm结果位于`./osm/`，生成的最终xodr地图位于`./xodr/`