
..数据还原:

=====================================
无监督降维
=====================================

如果你的功能数量很多，在监督步骤之前，可以通过无监督的步骤来减少功能.
很多的：引用：'无人值守学习'方法实现一个 'transform'方法可以用来降低维度.
下面我们将讨论大量使用这种模式的两个具体示例.

.. 主题:: **流水线技术**
    无监督数据简化和监督化估计器可以一步链接.参见: ref: 'pipeline'.

.. 当前模块:: sklearn

PCA: 主成分分析
----------------------------------

:class:'分解.PAC' 寻找能够捕捉原始特征的差异的特征的组合. 参见: ref: 'decompositions'.

.. 主题:: **示例**

   * :ref: 'sphx_glr_auto_examples_applications_plot_face_recognition.py'

随机投影
-------------------

模块: :mod:'random_projection' 提供了几种用于通过随机投影减少数据的工具.
请参阅文档的相关部分: : ref: 'random_projection'.

.. 主题:: **示例**

   * :ref:`sphx_glr_auto_examples_plot_johnson_lindenstrauss_bound.py`

特征征集
------------------------

:class:'cluster.FeatureAgglomeration' 适用
:ref: 'hierarchical_clustering' 将行为类似的功能分组在一起

.. topic:: **示例**

   * :ref:`sphx_glr_auto_examples_cluster_plot_feature_agglomeration_vs_univariate_selection.py`
   * :ref:`sphx_glr_auto_examples_cluster_plot_digits_agglomeration.py`

.. topic:: **特征缩放**

   请注意，如果功能具有非常不同的缩放或统计属性，则: class: 'cluster.FeatureAgglomeration'
   可能无法捕获相关功能之间的链接.使用a: class: 'preprocessing.StandardScaler' 可以在这些
   设置中使用.

