# - 🎇代码测试（30min）-
从下面的代码题目中，选择任意一个，用30min尝试解决。

*1* 算法类题目，选自力扣(LeetCode)经典题目，请在无AI支持下尝试解决；
*2* 应用类题目，基于GitHub开源代码进行简单的二次开发，可以使用任意AI工具辅助编程。

请共享屏幕，打开任意本地IDE，设计代码并运行测试。

## 1、算法类题目

**🎯 任务目标：**
给定一个二维数组，请返回「螺旋遍历」该数组的结果。

「螺旋遍历」：即顺时针遍历元素。从左上角开始，按照 ”向右、向下、向左、向上” 的顺序依次提取元素，然后再进入内部一层重复相同的步骤，直到提取完所有元素。

    例如：  
    输入：[1, 2, 3] [4, 5, 6] [7, 8, 9]
    输出：[1, 2, 3, 6, 9, 8, 7, 4, 5]


## 2、应用类题目

**🎯 任务目标：** 

基于 Camel-AI 框架，让 Agent 调用自定义的 tool，对 prompt 做出回答
##

**📋 参考步骤：**

step 1. 打开 Camel-AI 项目，配置环境，安装 camel
        
        项目地址：https://github.com/camel-ai/camel

step 2. 查看 examples / toolkits / human_toolkit.py , 

        理解代码中 
        
        **创建Toolkit** — **创建Model** — **创建Agent — Agent 调用 Model 和 Toolkit 完成任务**  

        的工作流程

step 3. 查看 camel / toolkits / human_toolkit.py , 代码中给出了 toolkit 的设计方式

step 4. 定义一个 OUR_toolkit(在一个单独的py文件中进行定义), 让 Agent 使用 

step 5. 使用 OUR_toolkit 完成指定任务
##

**💡Tips：**

1、创建 Model 时，需要通过 API 调用的方式，如果您没有可用的 API，可以使用下面这个免费的 API (来自ModelScope) ：

    - model_platform ：ModelScope
    - model_type ：可在 camel / types / enums.py 中，查看 ModelType 类，
                   选择一个支持的模型，比如 "Qwen/Qwen2.5-14B-Instruct" 等   
    - api_key ：ms-7e66d102-bb98-4eeb-9240-45dc32f88889

2、建议使用 python 3.10~3.12 版本
    

