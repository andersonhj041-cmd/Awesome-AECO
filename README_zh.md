# Awesome AECO [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[English](README.md)

AECO 代表建筑、工程、施工和运营（Architecture, Engineering, Construction, and Operations）。它指的是从最初设计到持续维护和运营的整个生命周期中，设计、建造和管理建筑或基础设施项目的集成过程。这一过程涉及多个学科的协同工作，以创建和管理建成环境。


> 精选的 AECO 资源、工具和技术列表。
> 受 [Awesome](https://github.com/sindresorhus/awesome) 启发。

## 目录

- [Awesome AECO](#awesome-aeco-)
  - [目录](#目录)
  - [BIM (建筑信息模型)](#bim-建筑信息模型)
  - [CAD (计算机辅助设计)](#cad-计算机辅助设计)
  - [Revit 插件与扩展](#revit-插件与扩展)
  - [模拟与分析](#模拟与分析)
  - [参数化与计算设计](#参数化与计算设计)
  - [物联网与智能建筑](#物联网与智能建筑)
  - [设施与资产管理](#设施与资产管理)
  - [生成式设计](#生成式设计)
  - [建筑自动化与机器人](#建筑自动化与机器人)
  - [数字孪生](#数字孪生)
  - [GIS 与制图](#gis-与制图)
  - [项目管理](#项目管理)
  - [贡献](#贡献)

---

## BIM (建筑信息模型)

- **IfcOpenShell**
  用于 BuildingSMART IFC 文件的开源工具包和几何引擎。支持通过 C++ 库和 Python API 读取、写入和修改 BIM 模型。
  *GitHub: [IfcOpenShell/IfcOpenShell](https://github.com/IfcOpenShell/IfcOpenShell)*

- **xBIM Toolkit**
  适用于 .NET 的可扩展 BIM 工具包，提供处理 IFC 数据（读取、创建、验证）的库。允许 Microsoft 技术栈的开发人员构建 BIM 应用程序。
  *GitHub: [xBimTeam/XbimEssentials](https://github.com/xBimTeam/XbimEssentials)*

- **BIMserver**
  开源 BIM 服务器平台（Java），使用 IFC 存储和管理建筑模型。作为一个具有版本控制和多用户协作功能的模型数据库。
  *GitHub: [opensourceBIM/BIMserver](https://github.com/opensourceBIM/BIMserver)*

- **IFC.js**
  用于将 IFC BIM 数据引入 Web 应用程序的 JavaScript 工具包（由 WASM 驱动）。包括用于快速解析的 `web-ifc` 和用于在 Three.js 中查看的 `web-ifc-three`。
  *GitHub: [ThatOpen/engine_web-ifc](https://github.com/ThatOpen/engine_web-ifc)*

- **That Open Engine Fragments**
  高性能 3D 引擎，使用 Fragments 格式高效处理海量 BIM 数据。
  *GitHub: [ThatOpen/engine_fragment](https://github.com/ThatOpen/engine_fragment)*

- **That Open UI Components**
  为建筑信息模型 (BIM) 应用程序设计的 Web 组件集合。
  *GitHub: [ThatOpen/engine_ui-components](https://github.com/ThatOpen/engine_ui-components)*

- **Speckle**
  开源 AEC 数据平台（“BIM 版 Git”），通过在设计工具之间流式传输几何图形和数据，实现实时协作和互操作性。
  *GitHub: [specklesystems/speckle-server](https://github.com/specklesystems/speckle-server)*

- **BHoM (Buildings and Habitats object Model)**
  建筑环境的协作计算框架和数据架构。定义了 AEC 领域（结构、环境、机电等）的核心对象模型。
  *GitHub: [BHoM/BHoM](https://github.com/BHoM/BHoM)*

- **Revit API Samples**
  Autodesk 官方仓库，演示了用于自动化和插件开发的 Revit API 用法。
  *GitHub: [Autodesk/revit-api](https://github.com/Autodesk/revit-api)*

- **BIMsurfer**
  基于 Web 的 IFC 模型查看器，具有碰撞检测和协作功能。
  *GitHub: [opensourceBIM/BIMsurfer](https://github.com/opensourceBIM/BIMsurfer)*

- **GomeraX**
  带有 AI 驱动 BIM 助手的实验性 IFC 查看器。具有 WebGL 和 WebGPU 渲染、高级剖切、第一人称导航、图元聚类以及通过本地大语言模型进行模型交互的自然语言命令功能。
  *GitHub: [salpbes/GomeraX](https://github.com/salpbes/GomeraX)*

- **.bim (dotBIM)**
  极简主义的 BIM 文件格式。
  *GitHub: [paireks/dotbim](https://github.com/paireks/dotbim)*

- **xeokit convert**
  使用 JavaScript 直接将 BIM 和 AEC 模型转换为 XKT 文件，以便在 xeokit 中实现超快加载。
  *GitHub: [xeokit/xeokit-convert/](https://github.com/xeokit/xeokit-convert/)*

- **xeokit BIM Viewer**
  基于 xeokit SDK 构建的捆绑式 BIM 查看器，具有测量、树状图浏览器、注释、切片、第一人称导航等功能。
  *GitHub: [xeokit/xeokit-bim-viewer](https://github.com/xeokit/xeokit-bim-viewer)*

- **xeokit SDK**
  高效的开源 JavaScript SDK 和 3D 引擎，拥有自己的 WebGL 渲染器和丰富的示例库，用于查看 BIM、IFC、BCF、Revit、点云等，支持真实世界坐标和 XKT 格式的双精度。
  *GitHub: [xeokit/xeokit-sdk](https://github.com/xeokit/xeokit-sdk)*

- **IFClite**
  用于在浏览器、服务器或桌面应用程序中处理 IFC 文件的开源工具包。具有 WebGPU 3D 查看器、IFC4/IFC4X3 支持、BCF 协作、IDS 合规性检查、bSDD 查找、2D 图纸生成以及导出为 IFC、glTF、CSV、JSON 和 Parquet 的功能。
  *GitHub: [louistrue/ifc-lite](https://github.com/louistrue/ifc-lite)*

## CAD (计算机辅助设计)

- **FreeCAD**
  免费、开源的参数化 3D CAD 建模器，采用模块化架构。包含用于 BIM 的 Arch 工作台，并支持导出为 IFC、DWG 和 STEP。
  *GitHub: [FreeCAD/FreeCAD](https://github.com/FreeCAD/FreeCAD)*

- **LibreCAD**
  基于 QCAD 社区版的开源 2D CAD 绘图工具。提供支持 DXF/DWG 的跨平台绘图 GUI。
  *GitHub: [LibreCAD/LibreCAD](https://github.com/LibreCAD/LibreCAD)*

- **BRL-CAD**
  成熟的开源实体建模系统，具有强大的 CSG 几何引擎和高性能光线追踪功能。
  *GitHub: [BRL-CAD/brlcad](https://github.com/BRL-CAD/brlcad)*

- **OpenSCAD**
  “程序员的实体 3D CAD 建模器”。用户通过编写定义基元和布尔运算的脚本来创建 3D 模型。
  *GitHub: [openscad/openscad](https://github.com/openscad/openscad)*

- **SolveSpace**
  一款轻量级的参数化 2D/3D CAD 程序，支持基于约束的草图绘制，并可导出为 STEP/DXF/STL。
  *GitHub: [solvespace/solvespace](https://github.com/solvespace/solvespace)*

- **CadQuery**
  基于 Python 的参数化 CAD 脚本框架，用于机械和建筑设计。
  *GitHub: [CadQuery/cadquery](https://github.com/CadQuery/cadquery)*

## Revit 插件与扩展

- **pyRevit**
  Autodesk Revit 的快速开发环境。允许用户使用 IronPython 或 CPython 通过扩展 API 创建自定义工具。
  *GitHub: [pyrevitlabs/pyRevit](https://github.com/pyrevitlabs/pyRevit)*

- **RevitLookup**
  Revit 的交互式 BIM 数据库浏览器。实时检查所选图元的数据（参数、属性）。
  *GitHub: [jeremytammik/RevitLookup](https://github.com/jeremytammik/RevitLookup)*

- **Rhino.Inside Revit**
  将 McNeel Rhino 3D 和 Grasshopper 嵌入 Revit 环境中，实现几何图形和参数的无缝传输。
  *GitHub: [mcneel/rhino.inside-revit](https://github.com/mcneel/rhino.inside-revit)*

- **IFC Exporter for Revit**
  Revit 使用的开源 IFC 插件，用于改进对 IFC (IFC2x3/IFC4) 的支持。
  *GitHub: [Autodesk/revit-ifc](https://github.com/Autodesk/revit-ifc)*

## 模拟与分析

- **EnergyPlus**
  美国能源部 (DOE) 旗舰级的全建筑能量模拟引擎。模拟加热/冷却负荷、HVAC 系统和能源消耗。
  *GitHub: [NREL/EnergyPlus](https://github.com/NREL/EnergyPlus)*

- **OpenStudio**
  位于 EnergyPlus 之上的全建筑能量建模跨平台工具集。
  *GitHub: [NREL/OpenStudio](https://github.com/NREL/OpenStudio)*

- **Ladybug Tools**
  开源环境分析工具套件，将 CAD 建模连接到物理引擎（例如，用于太阳能分析的 Ladybug，用于能量/采光的 Honeybee）。
  *GitHub: [ladybug-tools/ladybug](https://github.com/ladybug-tools/ladybug)*

- **Radiance**
  用于评估日光和电照明的行业标准照明模拟套件，可产生准确的亮度值。
  *GitHub: [LBNL-ETA/Radiance](https://github.com/LBNL-ETA/Radiance)*

- **OpenFOAM**
  用于气流和热模拟的计算流体动力学 (CFD) 工具包。
  *GitHub: [OpenFOAM/OpenFOAM-dev](https://github.com/OpenFOAM/OpenFOAM-dev)*

- **OpenSees**
  地震工程模拟开放系统。用于结构有限元分析 (FEA) 和结构地震模拟的框架。
  *GitHub: [OpenSees/OpenSees](https://github.com/OpenSees/OpenSees)*

## 参数化与计算设计

- **Dynamo**
  用于设计自动化的开源可视化编程平台。在 BIM 中常用于生成式设计和自动化重复性任务。
  *GitHub: [DynamoDS/Dynamo](https://github.com/DynamoDS/Dynamo)*

- **COMPAS**
  基于 Python 的计算框架，用于建筑、工程和数字制造。
  *GitHub: [compas-dev/compas](https://github.com/compas-dev/compas)*

- **Rhino.Compute**
  基于 Rhino 3D 几何内核的 REST 几何服务器。允许以编程方式无界面访问 Rhino 的建模能力。
  *GitHub: [mcneel/compute.rhino3d](https://github.com/mcneel/compute.rhino3d)*

- **BlenderBIM**
  用于 BIM 工作流程的 Blender 插件，支持 IFC 导入/导出和参数化建模。
  *GitHub: [blenderbim/blenderbim](https://github.com/blenderbim/blenderbim)*

- **Grasshopper-IFC**
  用于在 Rhino 中生成符合 IFC 标准的几何图形的 Grasshopper 插件。
  *GitHub: [MadsHolten/IFC-Grasshopper](https://github.com/MadsHolten/IFC-Grasshopper)*

- **Polygonjs**
  基于节点的 WebGL 设计工具，无需编码即可创建交互式 3D 体验和数字孪生。
  *GitHub: [polygonjs/polygonjs](https://github.com/polygonjs/polygonjs)*

## 物联网与智能建筑

- **Home Assistant**
  专注于本地控制和隐私的智能家居自动化和物联网设备集成平台。
  *GitHub: [home-assistant/core](https://github.com/home-assistant/core)*

- **openHAB**
  用于集成和控制智能建筑设备的供应商无关开源软件。
  *GitHub: [openhab/openhab-addons](https://github.com/openhab/openhab-addons)*

- **Eclipse VOLTTRON**
  建筑系统分布式传感和控制平台。提供从建筑设备收集实时数据的服务。
  *GitHub: [VOLTTRON/volttron](https://github.com/VOLTTRON/volttron)*

- **EdgeX Foundry**
  用于管理智能建筑中传感器和数据的模块化物联网平台。
  *GitHub: [edgexfoundry/edgex-go](https://github.com/edgexfoundry/edgex-go)*

- **ThingsBoard**
  用于设备管理、数据可视化和分析的开源物联网平台。
  *GitHub: [thingsboard/thingsboard](https://github.com/thingsboard/thingsboard)*

- **Google Digital Buildings**
  用于表示建筑及其安装设备的结构化信息的统一架构和工具集。
  *GitHub: [google/digitalbuildings](https://github.com/google/digitalbuildings)*

- **Brick Schema**
  开源统一元数据架构，用于高效表示建筑中的元数据。
  *GitHub: [BrickSchema/Brick](https://github.com/BrickSchema/Brick)*

## 设施与资产管理

- **Condo**
  用于跟踪维护工单、居民联系和费用支付的开源物业管理 SaaS。
  *GitHub: [open-condo-software/condo](https://github.com/open-condo-software/condo)*

- **Atlas CMMS**
  自托管的计算机化维护管理系统。允许团队安排工作订单并管理库存。
  *GitHub: [Grashjs/cmms](https://github.com/Grashjs/cmms)*

## 生成式设计

- **Anton**
  利用拓扑优化作为找形方法的 Blender 生成式设计框架。
  *GitHub: [senthurayyappan/anton](https://github.com/senthurayyappan/anton)*

- **Design Explorer**
  用于探索多维设计空间的 Web 应用程序，用于可视化参数化研究中的选项。
  *GitHub: [tt-acm/DesignExplorer](https://github.com/tt-acm/DesignExplorer)*

## 建筑自动化与机器人

- **ROS (Robot Operating System)**
  领先的机器人中间件，在 AEC 中用于原型设计建筑机器人或自动化设备。
  *GitHub: [ros/ros](https://github.com/ros/ros)*

- **Gazebo Simulator**
  高保真 3D 机器人模拟器，用于虚拟测试建筑机器人或自动化设备。
  *GitHub: [gazebosim/gz-sim](https://github.com/gazebosim/gz-sim)*

## 数字孪生

- **iTwin.js**
  Bentley 的开源库，用于创建和可视化基础设施数字孪生。
  *GitHub: [iTwin/itwinjs-core](https://github.com/iTwin/itwinjs-core)*

- **Digital Twin Toolkit**
  创建建筑和基础设施数字孪生的框架。
  *GitHub: [digitaltwinconsortium/DigitalTwinToolkit](https://github.com/digitaltwinconsortium/DigitalTwinToolkit)*

- **PlayCanvas**
  开源 WebGL 游戏引擎，用于构建交互式 3D 可视化和数字孪生。
  *GitHub: [playcanvas/engine](https://github.com/playcanvas/engine)*

## GIS 与制图

- **QGIS**
  免费、开源的 GIS，用于查看、编辑和分析地理空间数据。
  *GitHub: [qgis/QGIS](https://github.com/qgis/QGIS)*

- **CesiumJS**
  用于 3D 地球和地图可视化的 JavaScript 库，能够在地理空间背景下流式传输 BIM 数据。
  *GitHub: [CesiumGS/cesium](https://github.com/CesiumGS/cesium)*

- **OpenLayers**
  高性能 JS 库，用于 Web 上的交互式地图。
  *GitHub: [openlayers/openlayers](https://github.com/openlayers/openlayers)*

- **BlenderGIS**
  Blender 插件，在 Blender 的 3D 数据和 2D 地理数据之间架起桥梁。
  *GitHub: [domlysz/BlenderGIS](https://github.com/domlysz/BlenderGIS)*

- **Awesome GIS**
  精选的 GIS、遥感、3D 扫描和其他地理空间相关资源列表。
  *GitHub: [sshuair/awesome-gis](https://github.com/sshuair/awesome-gis)*

## 项目管理

- **OpenProject**
  具有甘特图、敏捷工作流和 BIM 集成功能的协作式项目管理工具。
  *GitHub: [opf/openproject](https://github.com/opf/openproject)*

- **LibrePlan**
  建筑项目的资源规划和进度安排软件。
  *GitHub: [LibrePlan/libreplan](https://github.com/LibrePlan/libreplan)*

## 贡献

欢迎贡献！请先阅读[贡献指南](contributing_zh.md)。
