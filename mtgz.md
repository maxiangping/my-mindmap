
2023-1-3
1.君智bug修复 
1.1 fix #2724 图表设计-折线图样式及交互优化
1.2 fix el-cascader移动端样式问题
2.君智内部系统换logo


移动端问卷选省市区，键盘弹起后下拉框定位不对

import { PredictionChart } from './predictionChart'

2023-1-4
1.预测预判
1.1 feat 特性图谱开发：图表展示、编辑、下载
1.2 feat 特性图谱接口联调：数据获取，数据刷新

2023-1-5
1.预测预判
1.1 feat 特性图谱不同节点个数，展示样式修改
1.2 fix 词云分析关键词字体大小修改

2023-1-6
1.君智上线
1.1 配合君智上线
1.2 fix 默认报告版本号问题修复
1.3 fix #2769 【生产环境】智能搜索，关系图谱时间筛选框没有居中，建议优化

本周工作：
1.预测预判-特性图谱开发：图谱展示、编辑、下载
2.预测预判-特性图谱接口联调：数据获取，数据刷新
3.词云分析-关键词字体大小修改
4.配合君智上线


2023-01-16
1.遍历树节点父节点的速度优化


2023-01-17
1. nginx websocket 请求超时时长配置
2. 舆情主题请求时长http和ws对比


2023-01-18
1. fix 自定义主题-热词分布切换到饼状图、柱状图、条形图只显示一半的视图修复
2.舆情主题http和ws请求时长对比

2023-01-19
1.舆情主题内部切换tab减少websocket连接

本周周报：
1、【热搜监测】整体概况-信息最高渠道展示错误修复 100%
2、【问卷作答】问卷描述清空后，答卷页依旧显示默认值修复 100%
3、【报告设计】遍历树节点获取父节点公共代码速度提升 100%
4、【配置修改】nginx请求超时时长配置 100%
5、【舆情主题】请求时长http和websocket对比(差别不大) 100%
6、【自定义主题】热词分布切换到饼状图、柱状图、条形图只显示一半的视图修复 100%
7、【舆情主题】切换内部tab，减少 websocket连接 100%
8、公共消息提示框显示关闭按钮 100%

下周工作计划：
1、配合君智修复问卷反馈问题
2、配合君智解决uat问题


2023-01-20
1.公共消息弹框加删除按钮

1.舆情接口页面加载数据慢，是否可以用同一个websocket解决（解决）
2.仪表板页面重复调用familyTree接口，查看可优化的地方（缓存）（解决）
3.websocket未登录不需要加载一次，页面总会报错（解决）
4.切换登陆用户后，原本的页面并不是最新的用户，权限未更新（解决）
5.舆情列表数据双滚动条特别慢（解决）
6.右上角下拉触点问题（解决）
7.调研报告数据源组合问卷不能正常生成图表（解决）


2023-01-30
1.公共消息弹框加删除按钮，部分问题修复
2.websocket未登录不需要加载一次，页面总会报错修复

2023-01-31
1.fix 舆情主题详情报表，全局筛选时间不生效修复
2.切换登陆用户后，原本的页面并不是最新的用户，权限未更新（解决）

2023-02-01
1.fix #2763 图表设计优化

2023-02-02
1.fix 中式报表样式修改

2023-02-03
1.仪表盘图表更新成Ant-G2plot组件，图表样式兼容 50%

本周周报：
1.公共消息弹框加删除按钮，部分问题修复 100%
2.未登录或者token过期情况下websocket不需要连接，不然页面总会报错修复 100% 
3.【舆情主题】详情报表，全局筛选时间不生效修复 100%
4.切换登陆用户后，原本的页面并不是最新的用户，权限未更新修复 100% 
5.君智反馈问题：图表设计优化、中式报表样式修改 100%
6.仪表盘图表更新成Ant-G2plot组件，图表样式兼容 50%

下周工作计划：
1、配合君智修复问卷反馈问题
2、配合君智解决uat问题


2023-02-06
1.仪表盘图表更新成Ant-G2plot组件，图表样式兼容 100%

2023-02-07
1. fix 滚动折线图图例的透明度等样式修改

vite构建
中式报表替换方案 
图表替换g2地图替换

2023-02-08
1.考核评价问卷原型评审
2.考核评价问卷-多选题开发 40%

2023-02-09
1.考核评价问卷-多选题开发 100%
2.fix alert弹框在移动端样式修改
3. 考核报表展示

多选题开发：
1.左侧列表新加多选题型、加数据结构(解决) 
2.标签：加分、减分 (解决) 
3.说明：显示方式和按钮文案；预览界面弹框说明 (解决)
4.分组设置：添加分组、删除分组、数据结构(解决)
5.允许填空设置：新增填空、删除填空、修改填空、展示填空、提交填空  (解决)
6.横向排列两列 (解决)

题目配置加字段：

optionList: [
	{
		optionDescribeType: number // 描述显示方式：1 直接显示在问卷页面 2 点击按钮后在弹窗中显示
		optionDescribeBtnTitle: string // 按钮显示文案
		inputOptions: [ //允许填空设置
			{	
				inputId: string // 填空项id
				inputTitle: string // 填空项标题
				inputPlaceholder: string // 填空项提示文案
			},
			{	
				inputId: string // 填空项id
				inputTitle: string // 填空项标题
				inputPlaceholder: string // 填空项提示文案
			}
		],
		scoreType: number // 标签：1 加分 0 减分
	}
]
optionGroup: [ // 分组设置
	{
		groupId: string // 分组id
		groupName: string // 分组名称
		groupOptions: [ 'optionId', 'optionId' ] // 分组选项
	},
	{
		groupId: string // 分组id
		groupName: string // 分组名称
		groupOptions: [ 'optionId', 'optionId' ] // 分组选项
	},
]


icon/datasource/datacollection/tab_fieldset.svg


1.仪表盘图表更新成Ant-G2plot组件，图表样式兼容 100%
2.滚动折线图图例的透明度等样式修改 100%
3.考核评价问卷原型评审
4.考核评价问卷-多选题开发、自增题型开发、查看下载答卷开发、报表统计开发 100%
5.配合考核评价问卷上线

https://blog.csdn.net/lee576/article/details/128222764



字体间距调整大小 0.5
字体调整  0.5
添加背景图片 1
文字自适应填充画布 0.5
添加模版样式，选择模版样式 1







思源黑体

font-family: 'Noto Sans CJK SC', 'Noto Sans CJK', 'Source Han Sans', source-han-sans-simplified-c, sans-serif;

这样声明可以让浏览器先调用系统内已安装的思源黑体，没有的话再从网络上加载。如果网络也加载失败，会回落到系统默认的非衬线字体。思源黑体的内置西文是 Adobe Source Sans Pro。

思源黑体 + Google Noto Sans

font-family: 'Noto', 'Noto Sans CJK SC', 'Noto Sans CJK', 'Source Han Sans', source-han-sans-simplified-c, sans-serif;

思源宋体


font-family: 'Noto Serif CJK SC', 'Noto Serif CJK', 'Source Han Serif SC', ‘ Source Han Serif ’ , source-han-serif-sc, serif;

思源宋体内置的西文字体是 Adobe Source Serif。

思源宋体 + Google Noto Serif

font-family: 'Noto Serif', 'Noto Serif CJK SC', 'Noto Serif CJK', 'Source Han Serif SC', ‘ Source Han Serif ’ , source-han-serif-sc, serif;

2023-02-10
1. fix 选项标题是空格就对选项隐藏
2. fix 考核报表筛选加搜索
3. fix 考核报表首次进去筛选条件默认选中第一个

2023-02-13
1.词云分析 
1.1 词云分析单词平铺空白
1.2 词云分析字体间距调整

        const canvasEl = elBox.value?.getElementsByTagName('canvas')?.[0]
        if(!isNull(canvasEl)) {
          console.log(canvasEl)
          const ctx = canvasEl.getContext("2d");
          const image = new Image()
          const imageType = props.chartsData.styles?.style ?? ''
          image.src = assetsLoader(`icon/datasource/chartdesign/wordcloud_cloud_temp.png`)
          image.onload = (_event) => {

              ctx?.drawImage(image, 500, 500, image.width, image.height)
              wordCloudChart.value?.update(chartOption.value as Partial<WordCloudOptions>)
          }
        }


2023-02-15
1.词云分析 
1. 词云字体加载
2. 词云平铺（字体大小调整）

问题：词云多次渲染


词云模版数据结构：
{
	tempId: number // 模版id
	tempName: string // 模版名称
	tempImageUrl: string // 模版示例图片
	tempStyles: string // 词云模版样式Json串
}

需要接口：
1. 模版新增接口
2. 模版列表接口
3. 单个模版根据Id查询详情接口


https://gw.alipayobjects.com
https://tracert.alipay.com
https://os.alipayobjects.com
https://zos.alipayobjects.com
https://www.yuque.com

2023-02-16
1.词云分析 
1.1 词云分析模版添加&提测
1.2 fix #2786 【词云分析】勾选文字内填充空白后，会出现卡顿的情况
1.3 配合词云上线
2.君智
2.1 fix 多选题填空自适应高度
2.2 fix 词云添加模版判断修改



iphone7  14.7.1
微信版本：8.0.32
微信部分手机有缓存的问题： 
location ~ .*\.(?:htm|html)$ {
    # 由于服务器部署多套项目环境，所以配置具体的项目目录。
    root    jimei-admin
    # 缓存设置 -1为永不缓存
    expires      -1;
    # 添加返回头字段，设置HTTP请求头
    add_header Cache-Control "private, no-store, no-cache, must-revalidate, proxy-revalidate";
}

 location ~* ^.+\.(css|js|txt|xml|swf|wav)$ {
          add_header Cache-Control no-cache;
  }

2023-02-17
1.知识工程平台
1.1 分享弹框开发 
1.2 分享答案页面开发
2.君智 
2.1 词云字体放大跨度加大，字体大小调整
2.2 词云放大缩小保存起来
2.3 fix 放大缩小保存到数据库中，下次进来再回显


中式报表需求疑问：
1.《工资条》报表有多个相同的表头？
2.《高新成本统计》匹配公式是怎么样
3.《分项目人力成本》最后一列'单个或多个月份‘是如何展示
4.《绩效上浮汇总表》合计和上浮占总比是页面计算吗
5.《社保公积金申报表》是两张报表还是一张

2023-02-20
1.君智词云 
1.1 词云遮罩背景
1.2 词云遮罩背景导出
2.sosmart
2.1 多选填空点击填空收起了多选题修复


'no-unnecessary-condition': 'on',


http://172.16.163.7:60001/questionnaire/share_answer_page/5RQFXbS0k8GjhDA6%2Fd6F%2BZlhq2mCpLtaOvY8s3JA4SCKvpCecSRr7ZPQkh7ze49CV36dT3IX3WJawGHODsYk3cxDkaN3hTTfxdl406s9tzbXBkrzqZlXeXOc%2BmnU%2Bnh7BsrSgBBgyowbpyAd7S%2FlIl8DA7nz8rXZ%2B5UOW37QBF%2BWBfOEWGhtNW78uNRvmndK


2023-02-21
1.君智词云提测
1.1 fix 多个重复分词导入只计算了一个词频
1.2 fix #2789 【词云分析】点击编辑/完成编辑按钮，不要刷新分词位置
1.3 fix 词云样式配置文案修改
1.4 fix 修改词云背景颜色

君智词云优化
1. 词云字体’编辑‘状态下点击’放大‘’缩小‘按钮跨度加大
2. 词云整体的’放大‘’缩小‘保存到后端接口，下次编辑可回显
3. 词云关键词小于10个就整体放大字体，其他情况正常显示
4. 词云添加背景颜色，添加背景导出正常


legacy({
        targets: [
          '> 1%, last 1 version, ie >= 11',
          'safari >= 10',
          'Android > 39',
          'Chrome >= 60',
          'Safari >= 10.1',
          'iOS >= 10.3',
          'Firefox >= 54',
          'Edge >= 15',
        ],
        polyfills: ['es.promise.finally', 'es/map', 'es/set'],
        modernPolyfills: ['es.promise.finally', 'es/global-this'],
      })

legacy({
        targets: ['defaults', 'not dead', 'Safari > 10.1', 'ios > 10.3'],
        renderLegacyChunks: false,
        modernPolyfills: ['es/global-this'],
      })


2023-02-22
1. sosmart评价系统过渡版
1.1 fix #2790 【答卷数据列表】无效和有效提示文案修改
1.2 fix 谷歌低版本浏览器打开分享答案页面表格无数据问题修复
2.君智词云修改
2.1 fix #2792 【词云分析】词云图形状背景尺寸按2560x1900分辨率适配
2.2 fix #2793 【词云分析】词云图形状背景颜色优化


字体放大的时候超出画布会消失
大字体的小字有时候点击不到
2.pdfmake
4.soflu文档学习


2023-02-23
1.君智词云修改 
1.1 fix #2791 【词云分析】选择关键词重复后词云图渲染速度优化
2.SoSmart系统
2.1 fix 多选题填空交互优化

SoFlu疑问：
1.函数库依赖什么情景下用到？
2.


本周工作内容 
1.【词云分析】新增需求的开发、提测
1.1. 词云字体’编辑‘状态下点击’放大‘’缩小‘按钮跨度加大
1.2. 词云整体的’放大‘’缩小‘保存到后端接口，下次编辑可回显
1.3. 词云关键词小于10个就整体放大字体，其他情况正常显示
1.4. 词云添加背景颜色，添加背景导出正常
1.5. 词云多个重复分词导入只计算了一个词频问题修复
1.6. 词云分析点击编辑/完成编辑按钮，不要刷新分词位置
1.7. 词云样式配置文案修改
1.8. 词云选择关键词重复后词云图渲染速度提升
2. 配合【词云分析】上线

下周工作计划
1.配合君智解决uat问题


2023-02-24
1.pdfmake转化方案学习
2.soflu文档学习
3.君智词云
3.1 词云背景不同尺寸兼容
3.2 fix #2794 词云分析字体顺序
3.3 fix #2795 【词云设计】词云编辑页面的生成模板按钮需隐藏

https://docs.editablejs.com/playground


2023-02-27 
1.soflu文档学习：输出精准营销方案
2.pdfmake学习:Editorjs转pdfmak实现demo

2023-02-28
1.soflu文档学习：输出精准营销方案
2.pdfmake学习:Editorjs转pdfmak实现demo

培训：
1.培梁主讲的《Web3.0》
2.乔宇主讲的《chat GPT》

2023-03-01 
1.soflu文档学习：输出精准营销方案（详细）
2.pdfmake学习:Editorjs转pdfmak实现demo

2023-03-02 
1.soflu文档学习：输出精准营销方案（详细）

2023-03-03
1.pdfmake学习:Editorjs转pdfmak实现demo


2023-03-06
1.soflu软件学习
2.内部风控君智系统(知识工程平台)
2.1 fix #2800 【问卷作答】作答页面的页眉调整为只在第一页展示
2.2 fix #2799 【问卷设计】段落说明新增样式功能



initStyle('title')
2023-03-07
1.soflu前后端交互学习
2.three.js模型交互学习
3.测试能力学习
4.pdfmake

2023-03-08
1.soflu和精准营销功能对比更新
2.知识工程平台 
2.1 fix #2801 【作答问卷】问卷分页，点击返回上一页按钮不需要校验题目是否填写。


2023-03-09
1.学习soflu函数 
2.3d学习
3.fork项目，清理大屏项目

大屏项目：Visual
fork账号：maxp
开发分支：qinghua/dev


2023-03-10
1.学习soflu函数 
2.3d学习
3.fork项目，清理君智项目

import { isEmpty } from '$system/functor'
function showToken() {
    if(isEmpty(this.globalVar.token)) return '未登陆'
    return this.globalVar.token
}

2023-03-13
1. editorjs 添加变量
2. 清理代码 qinghua/dev

2023-03-14
1. 清理代码 qinghua/dev

2023-03-15
1.富文本框插件-插入变量bug修复
2.大屏桌面应用搭建


70版本浏览器不能打开项目


大屏桌面应用：
https://tauri.app/zh-cn/
https://rsproxy.cn/



2023-03-16
1.中行： fix 客群画像图表创建客群添加客群规则
2.大屏桌面应用搭建

2023-03-17
1.大屏桌面应用搭建
2.输出文档： 《桌面应用集成大屏项目搭建步骤.docx》

2023-03-20
1.项目打包-低版本浏览器兼容


交叉分析筛选条件添加:
固定字段：
type: string // 调研人 'research_name'   地区 'interviewee_tel_province,interviewee_tel_city'
其他动态字段：
dynamicType：string // 姓名 'name'  手机号'phone' 地区'area' 其他字段 filed1 filed2 filed3...


填空题如果有观点用观点来分析bug


2023-03-21
1. 君智
1.1. fix #2805 【调研访谈】电话和线下调研，统计分析页面增加交叉分析
1.2. fix 默认报告刚添加观点的填空题在交叉分析中也显示分析bug修复
1.3. fix 电话问卷答卷中单选题、多选题的填空值没有回显bug修复
1.4. fix 交叉分析电话问卷的地区只查城市

2023-03-22
1. 请假

2023-03-23
1.SoFlu遇到问题文档整理

2023-03-24
1.昌飞项目开发&熟悉业务


2023-03-27
1.昌飞项目开发-文字转音频，音频转文字


2023-03-28
1.昌飞项目开发-接入麦克风
2023-03-29
1.昌飞项目开发-聊天接口联调
2023-03-30
1.昌飞项目开发-配合测试
2.帮助云创同事，搭建gitbook环境
2023-03-31
1.昌飞项目开发-配合测试


2023-04-03
1.wasm rust 加解密学习
BroadcastChannel
Background Tasks API
Beacon API

2023-04-04
1.fix 智能外呼页面加‘人工介入’按钮
2.知识图谱demo需求分析

2023-04-06
1.引入graphvis插件。类型声明等

1.股权穿透图
功能点： 开始动画，节点样式配置不一样，中心节点有label,鼠标经过节点显示label 并显示tooltips, 点击节点下钻，


2.树形股权图
功能点：树形，收起展开节点，鼠标经过节点显示label，收起展开节点后视图自适应 ，刷新，下载图片


3.关系图谱
功能点：开始动画，节点样式配置不一样，高亮当前节点的关联节点，显示当前点击节点配置，右键三个功能（编辑，删除，扩展节点），节点名称查询、路径查询


2023-04-07
1.君智 fix #2814 【问卷设计】矩阵多选题作答时非必填项为空时无法提交答卷
2.知识图谱demo开发


2023-04-10
1.君智交叉分析添加样本百分比需求修改&接口联调
2.知识图谱demo页的开发


2023-04-11
1.君智交叉分析添加样本百分比需求修改
1.1 fix 交叉分析样本百分比显示真实百分比
1.2 fix 交叉分析其他图表隐藏零数据计算值不对修复
1.3 fix 交叉分析表格高度自适应

2023-04-12
1. 知识图谱demo开发 40%
2023-04-13
1. 知识图谱demo开发 80%
2023-04-14
1. 知识图谱demo开发 100%

两周工作安排：
小静： 
 1. 本周一配合完成精准营销知识图谱demo展示
 2. 本周四下班之前实现关系图谱的配置（上左右的菜单栏），节点交互，并能保存到图表，和精准营销的知识图谱demo兼容（用切换图表类型的方式做）
 3. 周五实现和我这边的两个demo的交互，串联整个知识图谱搜索功能
 4. 每天登陆soflu至少2个小时，验证培梁给出的工作内容（下周二完成验证，周四完成验证报告）
我：
 1. 了解精准营销规则树需求内容，在下周三之前完成改版
 2. 本周五之前配合小静完成知识图谱demo,以及关系图谱在BI报表中的增删改查
 3. 每天登陆soflu至少2个小时，验证培梁给出的工作内容（下周二完成验证，周四完成写验证报告）

2023-04-17
1. 精准营销规则树需求了解
2. soflu验证功能，补充问题文档
2023-04-18
1. soflu验证功能，补充问题文档
2023-04-19
1. soflu验证功能，补充问题文档
2023-04-20
1. soflu验证功能，补充问题文档
2023-04-21
1. soflu验证功能，补充问题文档


play-circle


[
    {
        "nodeMouldId": 1,
        "nodeMouldName": "开始节点",
        "nodeMouldType": 1,
        "nodeMouldIcon": "play-circle"
    },
     {
        "nodeMouldId": 2,
        "nodeMouldName": "结束节点",
        "nodeMouldType": 2,
        "nodeMouldIcon": "pause-circle"
    }
]

2023-04-23
1. soflu验证功能，补充问题文档
2. 君智绩效考核分支加长请求超时时间

2023-04-24
1.规则树验证
2023-04-25
1.精准营销知识图谱下钻开发
2023-04-26
1.精准营销知识图谱下钻开发

演示大厅的浏览器弹出更新提示

公司 人物 属性
公司 10个 
人物 4个
bindToolBarEvent

stopLayout()

2023-05-04 
1.知识图谱demo组件图表设计和仪表板抽取成一个
2.股权穿透图样式修改
2.1. 拖动节点的时候不要乱动， 100%
2.2. 创建客群-用人名 100%
2.3. 跳转到决策流错乱 100%
2.4. 颜色配色修改 100%
2.5. 展开信息的背景颜色修改 100%
2.6. 收起信息不要背景颜色只要按钮 100%



249,149,38
134,166,255
52,167,241
27,195,194
230,210,100
229,101,97
199,142,35

2023-05-05 
1.股权穿透图样式修改
1.1. 右键点击-乱动 100%
1.2. 展开节点时不乱动 100%

SoFlu前端开发工具熟悉和使用并确定精准营销的细节功能能否实现

1、验证SoFlu功能
1.1、验证页面配置：页面缓存、页面动画、父子嵌套页面是否可以交互、页面的钩子函数等
1.2、验证能否动态监听变量、能否得到计算变量等
1.3、验证绑定事件的函数嵌套，以及函数执行的先后顺序如何实现
1.4、验证文件上传、文件下载、文件流解析等接口
2、验证导入源码、使用动态路由和源码共存的可行性
3、沟通精准营销后期开发方案

1、进一步熟悉（前端）全自动化开发平台开开发项目
2、5月26日之前验证动态路由和源码共存的可行性，验证SoFlu的功能覆盖是否支持精准营销开发的细节
3、沟通精准营销后期开发方案

完成精准营销产品功能实现

1、5月6日之前完成舆情图、上下游分析图、股权穿透图的开发和UI的调整
2、5月6日之前配合产品和组内成员实现柱状图、条形图、折线图、面积图、双Y轴、堆叠柱状图、堆叠条形图的自定义排序
3、沟通规则树改版的产品功能细节，并制定开发方案，预计5月22日之前完成

1、按计划完成精准营销的新加图谱功能
2、配合产品修改新加图谱的UI调整，交互调整
3、实现规则树的改版

2023-05-06
1.精准营销活动修改
1.1 fix 去掉成功标准节点的连线限制


1、SoFlu前端工具变量和样式使用
1.1、编写2套测试样式，使用变量抽取主题关变量，包括字体、字号、颜色等
1.2、使用全局变量，切换UI展示样式
1、验证SoFlu前端工具是否支持动态主题切换功能。

1、5月25日前完成图表下钻功能需求
1.1、完成报表设计多维度分析需求实现
1.2、完成图表设计部分数据下钻功能实现
1、完成图表设计所支持的图表数据下钻功能，包括二维表格、条形图、柱状图、折线图、面积图、饼图、地图、双Y轴图、堆叠柱状图、堆叠条形图、矩形树图等。
2、完成报表设计新增列维度，原维度变更为行维度。

2023-05-09
1.了解BI分析图表钻取的需求功能 

2023-05-10
1.了解BI分析图表钻取的需求功能 
2.精准营销demo调整

1.行列表格的数据结构 
2.数据下钻的交互



2023-05-11
1.精准营销demo调整
1.1.直接圈选高管将下面的子节点都可营销（解决）
1.2.双击去掉，表格加查看详情（解决）
1.3.展开侧边详细信息收起的按钮换掉（解决）


北京华清飞扬网络股份有限公司
上海卓易科技股份有限公司
{
"prop_name": "结算金额",
"prop_value": "--"
},
{
"prop_name": "结算比例",
"prop_value": "--"
},
下游结算


2023-05-15
1.精准营销知识图谱样式的修改
2.SoFlu前端工具变量和样式使用




SoFlu样式开发的局限性：
1.不支持像Less、Sass样式开发的样式变量
2.不支持多个全局样式文件的开发，一个项目全局样式只有一份
3.全局变量不能用在动态样式开发中，动态样式开发仅支持页面变量和参数变量


2023-05-16
1.精准营销知识图谱样式的修改

2023-05-17 
1.图表抖动的问题 
2.editorjs更新版本问题是否可以兼容
3.图表联动 做到解耦
4.vuex换成pinia


图表联动 做到解耦思路：
1.A图表的点击事件:图表设计中可配置是否可以点击，并可配置发送事件id
2.A抛出点击事件，并把点击值带出去，有些是单个维度，有些是多个维度（分表格、指标卡、事件轴、fusionchart、antv-g2plot几种类型的图表点击）
3.B接收点击事件，接收点击值：图表设计中可配置是否接收其他图表的点击事件，并可配置接收事件id
4.B做出相应的变化：数据改变、下钻、请求接口...

观察者模式


2023-05-18 
1.精准营销数字化营销需求时间评估
2.代码整理
3.SoSmart数智应用中心需求评审

2023-05-19 
1.精准营销实时营销需求开发：规则树开发
2.SoSmart数智应用中心前端时间评估


2023-05-22
1.完成事件属性、完成综合管理前端开发和接口联调

2023-05-23 
1.完成目标节点开发和接口联调
2.完成规则树（新建客群、客户分层）的开发

1.精准营销数字化营销4.3需求开发（总体35%）：完成规则树（新建客群、客户分层）、完成目标节点、完成事件属性、完成综合管理前端开发和接口联调
2.SoSmart数智应用中心时间评估、开发计划

2023-05-24 
1.offer节点 100%
2.响应标准、成功标准 50%

2023-05-25 
1.sosmart
2.响应标准、成功标准 100%




1.页面的布局以及页面图表配置config （头部、各个模块的box， 各个模块配置包括：标题，宽度，高度，子组件名称，是否有筛选条件)
2.所有图表用antv-g2plot 
3.大的公共模块：
3.1 考核评价分布、部门评价数排名、个人评价排名
3.2 考核因子、考核维度
3.3 各维度评价情况
3.4 点赞评价维度排名、点踩评价维度排名
4.小的公共模块：
4.1 考核维度刻度条
4.2 全局筛选条件
4.3 表格组件（树形、分页、筛选、下钻、标题、背景）
4.4 公司雷达-运营分析卡片
4.5 部门雷达-卡片
4.6 词云组件、环图组件、条形图组件、雷达图、仪表盘（同2）
4.7 分享 
4.8 导出
5.其他不能公用的模块
5.1 公司雷达：顶部轮询实时更新的汇总数据
5.2 个人雷达：顶部员工信息

其他需要注意的地方：
1.全局筛选条件是否禁用需要根据当前登录角色来决定
2.做页面的时候需要预留一个分享状态，如果是分享出来的页面，那么部分图表不可跳转


1.精准营销数字化营销4.3需求开发（总体60%）：完成实时节点前端开发和接口联调
2.SoSmart数智应用中心公共组件开发（总体前端80%）
2.1 表格组件开发（支持树形、分页可配置、筛选可配置、下钻跳转、标题可配置、背景可配置）
2.2 公司雷达-运营分析卡片
2.3 部门雷达-卡片
2.4 考核评价分布、部门评价数排名、个人评价排名
2.5 考核因子、考核维度
2.4 各维度评价情况（单元格合并表格）

2023-05-29
1. 精准营销完成实时节点前端开发和接口联调

2023-05-30 
1.表格组件开发（分页可配置、筛选可配置、下钻跳转）

2023-05-31 
1.表格组件开发（支持树形
2.考核因子、考核维度
3.各维度评价情况（单元格合并表格）


2023-06-01
1. 公司雷达-运营分析卡片
2. 部门雷达-卡片
3. 部门雷达-卡片-点击数据表格弹框

2023-06-02
1.考核评价分布、部门评价数排名、个人评价排名组件开发

2023-06-05
1.公司雷达：顶部轮询实时更新的汇总数据

2023-06-06
1.交互添加：数据筛选、数据下钻
2.精准营销： fix 事件属性管理的页面表格数据不展示


2023-06-08
1.公司雷达移动端页面开发
2023-06-09
1.公司雷达移动端页面开发
2023-06-12
1.部门雷达移动端调整
2.个人雷达移动端调整

2023-06-13
1. 公司雷达总数统计接口联调 60%

2023-06-14
1. 公司雷达总数统计接口联调
2. 君智线下问卷问题排查
3. 精准营销响应节点开发 


自动保存 和 正常保存




http://172.16.23.87:8100/reportplat/auth_failed?callback=%2FsystemManage
文档地址
http://172.16.163.8:4999/web/#/28?page_id=636

2023-06-15
1.响应节点开发和接口联调


2023-06-16
1.奖励节点开发和接口联调



${orderNo}  o.order_no like '%订单编号%' and
${checkName}  check_name = '检测人' and
${supplierName}   o.supplier_name = '供应商' and
oi.order_date>='${startDate}' 
and oi.order_date<='${endDate}'
${top}

测试环境页面地址：
供应商整体分析
http://172.16.163.5:8100/xnycustomer/supplier_analysis
采购对比分析
http://172.16.163.5:8100/xnycustomer/comparative_analysis
试用评价分析
http://172.16.163.5:8100/xnycustomer/trial_evaluation_analysis
订单管理
http://172.16.163.5:8100/xnycustomer/order_management

2023-06-18
1. 新能源订单管理页面开发

2023-06-19
1.新能源测试环境部署，配合测试修改问题
2.fix 新能源样式修改
3.fix 新能源项目图表数据不需要缓存
4.fix 新能源项目添加自定义图表字段排序
5.fix 新能源隐藏中式报表

{"ruleDay":7,"eventRule":"[{\"$and\":[{\"$and\":[{\"1@=\":[\"1\"]}]},{\"$and\":[{\"1@=\":[\"1\"]}]}]}]","eventName":"信用卡还款","eventRelation":"in"}




不等宽柱状图 1.5d
交叉表格 2d
瀑布图 0.5d
气泡图 0.5d
直方图 0.5d
总共：6d


eventName //事件类型
eventRuleEndTime //事件规则结束时间
eventRuleStartTime; //事件规则开始时间
eventRelation // 做过

2023-06-20
1.精准营销-渠道节点


2023-06-25
1.sosmart雷达看板接口联调-图表联动

2023-06-26
1.sosmart雷达看板接口联调-表格分页、词云分词


公司雷达图表。 本地bi地址
http://172.16.23.87:8100/reportplat/auth_failed?callback=%2FsystemManage
文档地址
http://172.16.163.8:4999/web/#/28?page_id=636


2023-06-27
1.sosmart雷达看板接口联调--表格筛选

1.条形图被切、条形图样式和设计稿不同
2.跳转页面：跳转部门 跳转个人
3.词云数据超过了遮罩图片
4.骨架屏 联动图表加载样式


172.16.23.87:11901   后端地址
172.16.23.87:8100     前端地址只调试图表使用的是自己造的测试数据

172.16.23.87:21901   后端地址
172.16.23.87:8800     前端地址
测试分词 单点登录 和SoSmart测试环境同步的数据

2023-06-28
1.sosmart雷达看板接口联调--部门看板-弹框表格接口
2.Sosmart加载数据添加骨架屏、联动图表加载样式


中式报表mixins 导入了很多小的文件，最好用异步加载组件的方式来做

2023-06-29
1、 精准营销：只要客户属性满足和事件满足、客群剔除有一个配置了规则就可以
2、sosmart雷达看板接口联调
2.1 切换tab强制重新渲染名字相同的组件
2.2 个人雷达的刻度条显示
2.3 评价维度排名回显
2.4 评价维度排名表格文案修改

2023-06-30
1、sosmart雷达看板H5样式调整

2023-07-05
1. 精准营销-响应节点样式修改
2.sosmart问题修复
2.1 fix #2848 【个人评论雷达】页面雷达图展示不全
2.2 fix #2846 【个人评价雷达】评价数据情况-评价数据显示错误


测试机权限还没申请下来可以先用下面几个地址在自己手机测一下页面交互：
公司雷达
https://kmind.feisuanyc.com:9443/smartboard/m/company_radar?authToken=64a76d596b81b851d855d316
部门雷达
https://kmind.feisuanyc.com:9443/smartboard/m/department_radar?authToken=64a76d596b81b851d855d316
个人雷达
https://kmind.feisuanyc.com:9443/smartboard/m/personal_radar?authToken=64a7c2556b81b851d855deca

64a4dd9a87a4ff2c78d761d5
2023-07-06
1.sosmart问题修复
1.1 fix #2869 【个人评价雷达】评价列表点击加载更多到最后一页时显示无数据
1.2 fix #2874 【部门管理雷达】个人评价情况-评价列表存在重复数据
1.3 fix 考核因子tips文案补充
1.4 fix #2887 【个人评价雷达】评价数据情况-部门和公司个人考核项排名合并成一个图表
1.5 fix #2903 【个人评价雷达】维度数据错误和样式异常
1.6 fix #2834 【公司管理】个人评价情况-个人评价排名
1.7 fix #2841 个人评价雷达-评价数据情况，当月评价他人次数与明细不一致
1.8 fix #2859 【公司管理雷达】排名图表样式显示错误
1.9 fix 表格行超出...ios兼容
1.10 fix #2904 【个人评价雷达】本人信息&评价情况-考核维度细项因子雷达和维度得分图表不显示
1.11 fix #2847 【个人评价雷达】表头与明细对应不上
1.12 fix #2897 【个人评价雷达】评价他人明细和评价他人次数不一致
1.13 fix #2913 【优化】【个人评价雷达】工作成果数据明细姓名、部门、岗位三个字段样式需调整
1.14 fix #2912 【个人评价雷达】评价明细-被评价数据明细无数据显示

加载更多被截掉

2023-07-07
1.sosmart问题修复
1.1.fix 当前登录人只有一个公司的权限的时候只能选中当前公司
1.2.fix 公司名称换行的问题
1.3 fix #2923 【优化】【个人评价雷达】评价明细--被评价数据明细表头与明细内容在iOS上错位
1.4 fix #2922 【公司管理雷达、部门管理雷达】点击部门或人员联动下方图表，切换到其他tab下还显示之前页面选择的部门或人员
1.5 fix #2924 【部门管理雷达】个人评价情况和考核项评价情况顺序替换
1.6 fix #2850 【优化】【公司管理雷达、部门管理雷达、个人评价雷达】评价列表新增【评价详情】页面
1.7 fix 个人总计数时间重叠
1.8 fix 环形图样式优化
1.9 fix #2925 【公司、部门、个人雷达】所有评价词云分布按关键词词频显示字体大小
1.10 fix #2926 【公司管理雷达】图表标题增加时间前缀
1.11 fix #2884 【优化】【部门管理雷达】总体评价情况-上月评价中的总数、点赞、点踩详情页中加载更多优化
1.12 fix #2895 【优化】环形图选中选择维度状态，点击一个维度，其它维度收起



-- 开发使用
http://10.8.240.92:8805/#/login?tenantId=system&appCode=bi&targetUrl=http://172.16.23.31:5173/m/department_radar
-- 测试使用
http://10.8.240.92:8805/#/login?tenantId=system&appCode=bi_test&targetUrl=http://172.16.163.5:8300/smartboard/m/personal_radar

2023-07-11
1.crm问题修复 
1.1 fix #2879 【活动设计】文件上传方式新建客群时，保持上传文件方框与字段匹配的方框高度保持一致
1.2 fix #2885 【活动设计】裂变营销节点提示优化
1.3 fix #2881 【活动设计】开始节点后支持连接历史名单
1.4 fix #2928 【活动设计】裂变营销节点裂变人数提示
1.5 fix #2932 【客户画像】新建客群时，客群类型在页面选择中没有决策流客群这个选项
1.6 fix #2935 【综合配置】保存时，客户查询字段不校验必须有唯一标识字段
1.7 fix 小屏幕适配
1.8 fix #2930 【综合配置】决策流程数据表配置，下方还有配置项，但是不能往下滚动
2.sosmart评价系统
2.1 fix 去掉雷达看板重复请求接口
2.2 fix 接口后缀加随机数


2023-7-12 
1.crm问题修复 
1.1 fix #2931 【活动设计】渠道节点上下左右不居中对齐
1.2 fix  #2933 【活动设计】事件属性满足优化
1.3 fix #2934 【活动设计】渠道节点触达时间不需要英文提示
1.4 fix #2936 【活动设计】目标客群节点标题合并与对齐
1.5 fix #2937 【活动设计】目标客群节点，新建客群通过存量导入客群方式导入规范、样式优化
1.6 fix #2940 【客户分群】客户分群列表页样式优化
1.7 fix #2939 【活动设计】营销活动列表页，样式优化
1.8 fix #2938 【客群分群】通过存量导入方式新建客群的导入规范和样式优化
1.9 fix #2929 【综合配置】选择客户主表时，二级选项显示表的别名
2.bi图表
分支创建

2023-7-13
1.bi数据分析
1. 瀑布图























	  