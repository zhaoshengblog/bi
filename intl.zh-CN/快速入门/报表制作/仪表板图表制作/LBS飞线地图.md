# LBS飞线地图 {#concept_pgm_jpv_k2b .concept}

如果您已经阅读过[仪表板概述](intl.zh-CN/快速入门/报表制作/仪表板概述.md#)和[仪表板基本操作](intl.zh-CN/快速入门/报表制作/仪表板基本操作.md#)，那么本章将为您介绍如何创建一个LBS飞线地图。如果您还需要对数据集做进一步的编辑，或者想重新创建一个数据集，请参阅[创建数据集](intl.zh-CN/快速入门/数据建模/管理数据集/编辑数据集.md#)。

LBS飞线地图以一个地图轮廓为背景，用动态的飞线反映两地或者多地之间的数据关系。

LBS飞线地图是由两个地理区域和LBS飞线度量构成的。地理区域由数据的维度决定，如省份或者城市；LBS飞线度量的大小由数据的度量决定，如运输成本，订单数量等。

## LBS飞线地图须知 {#section_pdr_xpv_k2b .section}

LBS飞线地图的地理区域最多只能取2个维度，并且维度类型必须为地理信息，如区域，省，城市等；LBS飞线度量区域最多取1个度量。

以下场景均以company\_sales\_record数据集为例。

**场景示例：用LBS飞线地图展示从各区域到各省份的运输成本。**

1.  登录Quick BI控制台。
2.  单击**数据集**，进入数据集管理页面。
3.  选择company\_sales\_record数据集，单击**新建仪表板**，进入仪表板编辑页面。
    -   如果您使用的是**标准版**或者**高级版**，页面会自动跳转到常规仪表板编辑页面。
    -   如果您使用的是**专业版**，需要您手动选择进入**常规模式**或者**全屏模式**。以下示例以**常规模式**为例。
4.  单击**LBS飞线地图**图标，LBS飞线地图的图例会自动显示在仪表板展示区。
5.  在数据标签页，为LBS飞线地图选择需要的维度字段和度量字段。

    在维度列表中，找到**区域**，并将其添加到地理区域/经纬度（from）区域中。找到**省份**，并将其添加到地理区域/经纬度（to）区域中。在度量列表中，找到**运输成本**，并将其添加到LBS飞线度量区域中，如下图所示。

    **说明：** 请确保区域字段和省份字段的维度类型已经从字符串切换为了地理信息。

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/15477/15382146076992_zh-CN.png)

6.  单击**更新**，系统自动更新图表。
7.  在样式标签页可更改图表的标题，布局和系列设置，如下图所示。

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/15477/15382146076993_zh-CN.png)

    在布局中，将地图底图设置为高德电子地图，并且将显示图例设置在图表下方，更新后的图表如下图所示。

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/15477/15382146076994_zh-CN.png)

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/15477/15382146076995_zh-CN.png)

    **说明：** 由于图表中的飞线是动态的，您还可以通过飞线时间来调整飞线的运动速度。数值越大，飞线的速度就越慢。

8.  单击**保存**图标，保存该仪表板。

    在图表右上方，选择**更多操作** \> **删除**，可删除当前图表。


有关各地区详细信息对照表请参见：[各地区详细信息对照表](http://docs-aliyun.cn-hangzhou.oss.aliyun-inc.com/assets/attach/48322/cn_zh/1534241743586/%E5%90%84%E5%9C%B0%E5%8C%BA%E8%AF%A6%E7%BB%86%E4%BF%A1%E6%81%AF%E5%AF%B9%E7%85%A7%E8%A1%A8.xls)。

