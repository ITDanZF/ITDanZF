<div align="center">

<img src="https://capsule-render.vercel.app/api?type=soft&color=0:0B1220,100:115E59&height=190&section=header&text=hejinyu&fontSize=68&fontColor=F8FAFC&fontAlignY=34&desc=AI%20%C2%B7%20WebGIS%20%C2%B7%20Drone%203D%20%C2%B7%20Digital%20Twin&descAlignY=62&descSize=16&descColor=CCFBF1" width="100%" alt="hejinyu" />

<a href="#zh-cn"><img alt="中文" src="https://img.shields.io/badge/%E4%B8%AD%E6%96%87-0F766E?style=for-the-badge" /></a>
&nbsp;
<a href="#en"><img alt="English" src="https://img.shields.io/badge/English-0B1220?style=for-the-badge" /></a>

</div>

<a id="zh-cn"></a>

<div align="center">

# hejinyu

**AI 应用开发工程师 / WebGIS 前端开发工程师**

无人机三维可视化 · 数字孪生 · AI 应用开发

[![Email](https://img.shields.io/badge/hejinyuhello%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:hejinyuhello@gmail.com)

</div>

我做两类前端里的空间产品，也做能交给人使用的 AI 应用。地图侧用 Cesium 把无人机航线、高度和地形关系画进三维地球；场景侧用 Three.js 做数字孪生里的模型编排。AI 侧用 TypeScript 把对话、工具和本地数据接成工作流，桌面端用 Electron，智能体用 LangChain 和 LangGraph。

## 三条业务线

<table>
  <tr>
    <td width="33%" valign="top">
      <h3 align="center">无人机三维可视化</h3>
      <p align="center">
        <img alt="CesiumJS" src="https://img.shields.io/badge/CesiumJS-6CADDF?style=flat-square&logo=cesium&logoColor=white" />
        <img alt="Vue" src="https://img.shields.io/badge/Vue-42B883?style=flat-square&logo=vuedotjs&logoColor=white" />
        <img alt="WebGIS" src="https://img.shields.io/badge/WebGIS-0F766E?style=flat-square" />
      </p>
      在三维地球上表达航点、航段和离地高度，服务无人机航线规划这类 WebGIS 前端。
    </td>
    <td width="33%" valign="top">
      <h3 align="center">数字孪生</h3>
      <p align="center">
        <img alt="Three.js" src="https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=threedotjs&logoColor=white" />
        <img alt="Next.js" src="https://img.shields.io/badge/Next.js-111111?style=flat-square&logo=nextdotjs&logoColor=white" />
        <img alt="GLB" src="https://img.shields.io/badge/GLB-5586A4?style=flat-square" />
      </p>
      把设备模型导入场景，管理资源，再对物体做平移、旋转和缩放。
    </td>
    <td width="34%" valign="top">
      <h3 align="center">AI 应用开发</h3>
      <p align="center">
        <img alt="LangChain" src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" />
        <img alt="LangGraph" src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square" />
        <img alt="Electron" src="https://img.shields.io/badge/Electron-47848F?style=flat-square&logo=electron&logoColor=white" />
      </p>
      把模型接进创作、建模和互动叙事，保留上下文、工具过程和本地数据。
    </td>
  </tr>
</table>

## 相关项目

### [DroneLine](https://github.com/ITDanZF/DroneLine) · 无人机航线的 WebGIS 前端

面向航线规划的三维地球场景，仓库说明对应司空类航线产品。航点用链表维护，只能从航线首尾继续延伸。空中航段用绿色自定义材质绘制，每个航点再落一条白色垂线到地形或椭球面，高度关系在场景里直接可见。当前示例是深圳附近的一条航线，航点高度 500 米，进入页面后相机会飞到起点。

`Vue 3` · `TypeScript` · `CesiumJS` · `Vite`

### [threeEditor](https://github.com/ITDanZF/threeEditor) · 数字孪生场景编辑

浏览器里的三维编辑器，用来把模型摆进孪生场景。可以导入 GLB，在文件树里管理资源，对物体平移、旋转、缩放。场景数据写在本地 IndexedDB。仓库里带了一个 GLB 设备模型，用来走通从导入到编辑的流程。

`Next.js` · `React Three Fiber` · `Three.js` · `Tailwind CSS`

### [Noteaide](https://github.com/ITDanZF/Noteaide) · 对话式三维建模

AI 三维建模智能体。使用者用自然语言描述模型，由助手创建和编辑，不把专业建模软件当作入口。首页讲清这个产品，应用内有独立的绘图对话页，并放了模型选择和深度思考入口。对话页已经接上，从描述到模型的闭环还在继续做。

`React` · `TypeScript` · `Vite` · `Three.js` · `Zustand`

### [StoryOS](https://github.com/ITDanZF/StoryOS) · 本地优先的 AI 应用

长篇小说的桌面工作台，用来说明一条完整的 AI 应用链路。书架管理书籍、分卷和章节，正文在分页编辑器里写，也可以打开阅读器。AI 按全书、项目或当前章节续写和改写；复杂任务会规划、执行、审查，影响较大的操作先预览再确认。项目、会话和运行记录存在本机 SQLite。模型可接 OpenAI、DeepSeek、通义千问，密钥由使用者自己配置。

`Electron` · `React` · `LangChain` · `LangGraph` · `Tiptap` · `SQLite`

### [alGalgame](https://github.com/ITDanZF/alGalgame) · AI 互动影像

实验性的 AI Galgame，仍在开发。产品结构是网页前端负责演出，服务侧连接语言模型、图像生成和向量记忆。服务端目前从 LangChain 这条线开始搭。

`TypeScript` · `Vue` · `LangChain`

[langchainjs-learn](https://github.com/ITDanZF/langchainjs-learn) 是配套练习：Node 示例、RAG 和向量检索。

## 常用技术

<p align="center">
  <img src="https://skillicons.dev/icons?i=ts,js,vue,react,nextjs,vite,threejs,electron,nodejs&perline=9" alt="TypeScript, JavaScript, Vue, React, Next.js, Vite, Three.js, Electron, Node.js" />
</p>

<p align="center">
  <img alt="CesiumJS" src="https://img.shields.io/badge/CesiumJS-6CADDF?style=for-the-badge&logo=cesium&logoColor=white" />
  <img alt="WebGL" src="https://img.shields.io/badge/WebGL-990000?style=for-the-badge&logo=webgl&logoColor=white" />
  <img alt="LangChain" src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" />
  <img alt="MySQL" src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
</p>

图形练习还包括 [react-vite-webgl](https://github.com/ITDanZF/react-vite-webgl)、[webgl](https://github.com/ITDanZF/webgl) 和 [opengl](https://github.com/ITDanZF/opengl)。

<div align="center">

[阅读英文 English](#en)

</div>

---

<a id="en"></a>

<div align="center">

# hejinyu

**AI Application Engineer / WebGIS Frontend Engineer**

Drone 3D visualization · Digital twins · AI applications

[![Email](https://img.shields.io/badge/hejinyuhello%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:hejinyuhello@gmail.com)

</div>

I build spatial products for drones and digital twins, and I also ship AI applications people can actually use. On the map side, Cesium draws routes, altitude, and terrain into a 3D globe. On the scene side, Three.js is where device models are placed and edited. On the AI side, TypeScript connects chat, tools, and local data. Desktop apps run on Electron. Agents run on LangChain and LangGraph.

## Three lines of work

<table>
  <tr>
    <td width="33%" valign="top">
      <h3 align="center">Drone 3D / WebGIS</h3>
      <p align="center">
        <img alt="CesiumJS" src="https://img.shields.io/badge/CesiumJS-6CADDF?style=flat-square&logo=cesium&logoColor=white" />
        <img alt="Vue" src="https://img.shields.io/badge/Vue-42B883?style=flat-square&logo=vuedotjs&logoColor=white" />
        <img alt="WebGIS" src="https://img.shields.io/badge/WebGIS-0F766E?style=flat-square" />
      </p>
      Waypoints, flight segments, and height above terrain, shown on a 3D globe for drone mission planning.
    </td>
    <td width="33%" valign="top">
      <h3 align="center">Digital twin</h3>
      <p align="center">
        <img alt="Three.js" src="https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=threedotjs&logoColor=white" />
        <img alt="Next.js" src="https://img.shields.io/badge/Next.js-111111?style=flat-square&logo=nextdotjs&logoColor=white" />
        <img alt="GLB" src="https://img.shields.io/badge/GLB-5586A4?style=flat-square" />
      </p>
      Import equipment models, organize them, then move, rotate, and scale them in the scene.
    </td>
    <td width="34%" valign="top">
      <h3 align="center">AI applications</h3>
      <p align="center">
        <img alt="LangChain" src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" />
        <img alt="LangGraph" src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square" />
        <img alt="Electron" src="https://img.shields.io/badge/Electron-47848F?style=flat-square&logo=electron&logoColor=white" />
      </p>
      Models wired into writing, 3D modeling, and interactive stories, with context, tools, and local data.
    </td>
  </tr>
</table>

## Selected projects

### [DroneLine](https://github.com/ITDanZF/DroneLine) · WebGIS frontend for drone routes

A 3D globe for route planning, aimed at the kind of flight-route product described in the repo. Waypoints live in a linked list and new segments attach only at the start or the end. Airborne segments use a green custom material. Each waypoint also drops a white line to the terrain, or to the ellipsoid when terrain is unavailable, so altitude stays visible. The sample route is near Shenzhen, with waypoints at 500 meters. The camera flies to the first point on load.

`Vue 3` · `TypeScript` · `CesiumJS` · `Vite`

### [threeEditor](https://github.com/ITDanZF/threeEditor) · Scene editor for digital twins

A browser editor for placing models into a twin scene. It imports GLB files, keeps them in a file tree, and translates, rotates, and scales the selection. Scene data is stored in local IndexedDB. The repo includes one equipment GLB so the path from import to edit can be tried end to end.

`Next.js` · `React Three Fiber` · `Three.js` · `Tailwind CSS`

### [Noteaide](https://github.com/ITDanZF/Noteaide) · Conversational 3D modeling

An AI agent for creating and editing 3D models in natural language. The product idea is that a person describes the model, and the assistant builds it, without starting from a professional modeling tool. The home page states that, and the app has a separate drawing chat with model selection and a deep-thinking entry. The chat surface is in place. The loop from description to a finished model is still being built.

`React` · `TypeScript` · `Vite` · `Three.js` · `Zustand`

### [StoryOS](https://github.com/ITDanZF/StoryOS) · A local-first AI application

A desktop workspace for long-form fiction, and a complete AI product path. A shelf holds books, volumes, and chapters. Writing happens in a paginated editor, with a reader for preview. The model can continue or rewrite from the book, the project, or the current chapter. Larger tasks are planned, executed, and reviewed. High-impact actions are previewed before they are approved. Projects, sessions, and runs stay in local SQLite. OpenAI, DeepSeek, and Qwen-compatible endpoints are supported, with keys supplied by the user.

`Electron` · `React` · `LangChain` · `LangGraph` · `Tiptap` · `SQLite`

### [alGalgame](https://github.com/ITDanZF/alGalgame) · AI interactive story

An experimental AI galgame, still in development. The web frontend handles the performance. The service side is meant to connect a language model, image generation, and vector memory. The server work currently starts from the LangChain directory.

`TypeScript` · `Vue` · `LangChain`

[langchainjs-learn](https://github.com/ITDanZF/langchainjs-learn) is the companion practice repo: Node examples, RAG, and vector search.

## Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=ts,js,vue,react,nextjs,vite,threejs,electron,nodejs&perline=9" alt="TypeScript, JavaScript, Vue, React, Next.js, Vite, Three.js, Electron, Node.js" />
</p>

<p align="center">
  <img alt="CesiumJS" src="https://img.shields.io/badge/CesiumJS-6CADDF?style=for-the-badge&logo=cesium&logoColor=white" />
  <img alt="WebGL" src="https://img.shields.io/badge/WebGL-990000?style=for-the-badge&logo=webgl&logoColor=white" />
  <img alt="LangChain" src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" />
  <img alt="MySQL" src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
</p>

Graphics practice also lives in [react-vite-webgl](https://github.com/ITDanZF/react-vite-webgl), [webgl](https://github.com/ITDanZF/webgl), and [opengl](https://github.com/ITDanZF/opengl).

<div align="center">

[阅读中文 Chinese](#zh-cn)

</div>

---

<div align="center" id="github">

<img height="165" alt="GitHub stats" src="https://github-readme-stats.vercel.app/api?username=ITDanZF&show_icons=true&theme=calm&hide_border=true&rank_icon=percentile" />
<img height="165" alt="Top languages" src="https://github-readme-stats.vercel.app/api/top-langs/?username=ITDanZF&layout=compact&theme=calm&hide_border=true&langs_count=8" />

[hejinyuhello@gmail.com](mailto:hejinyuhello@gmail.com)

</div>
