<h1> Refined Open WebUI Service Instance Deployment Document </h1>

<h2> Introduction to Open WebUI and Refined </h2>

<p>Open WebUI is a feature-rich and user-friendly self-hosted Web user interface (WebUI) designed to interact with large language models (LLMs), especially those supported by Ollama or services compatible with the OpenAI API. Open WebUI provides the ability to run completely offline, which means that users can talk to models without an internet connection, which is especially important for data privacy and security-sensitive application scenarios.
Here are some of the key features of Open WebUI:
Intuitive interface: Open WebUI's interface is inspired by ChatGPT, providing a clear and user-friendly chat interface that makes interaction with large language models intuitive.
2. Extensibility: This platform is extensible, meaning that it can be customized and enhanced by adding new plug-ins or features to adapt to different usage scenarios and needs.
3. Offline operation: Open WebUI supports completely offline operation, does not rely on network connection, and is suitable for use on any device, whether on an airplane or in remote areas.
Compatibility: It is compatible with multiple LLM runers, including Ollama and OpenAI APIs, which allows users to select and run different language models from multiple sources.
Self-hosted: Users can deploy Open WebUI on their own servers or devices, which provides greater protection for data privacy and control.
Markdown and LaTeX support: Open WebUI provides comprehensive Markdown and LaTeX functionality that allows users to generate rich text output, which is useful in scientific and academic communication.
Local RAG Integration: The Retrieval Enhanced Generation (RAG) feature allows the model to leverage locally stored data for more in-depth and specific responses, enhancing chat interactions.
Tongyi Bailian is an advanced multi-modal pre-training model launched by Alibaba Cloud. It combines natural language processing (NLP) and computer vision (CV) techniques to understand and generate many types of data, such as text, images, video, and more. The design goal of Tongyi Bailian is to provide developers and enterprises with a powerful tool for more efficient and intelligent data processing and analysis in various application scenarios. </p>

<p> this service integrates openwebui and refining, and provides ui service based on refining with one click </p>

<h2> Billing instructions </h2>

<p> The cost of the Open WebUI panel on Alibaba Cloud is mainly related:
* Specifications of the selected GPU cloud server
* Disk Capacity
* Internet bandwidth </p>

<p> Billing method: Pay-as-you-go (hourly) or package year and month
The estimated cost can be seen in real time when the instance is created. </p>

<p> Refined model call cost:
* When you open the Hundred Refinement for the first time, the platform will automatically issue exclusive free quotas for newcomers of each model. For more information, see <a href = "https://help.aliyun.com/zh/model-studio/new-free-quota?spm=a2c4g.11186623.help-menu-2400256.d_4_1.6dea55efFQCijR#view-quota"> Hundred Refinement Newcomer Free Quota </a>. </p>

<h2> Deployment Architecture </h2>

<p> The deployment architecture adopts ECS (cloud server) single-machine deployment </p>

<p><img width="600" src="architecture_ecs_single.png"/></p>

<h2> Permissions required for RAM accounts </h2>

<table>
<thead>
<tr>
<th> Permission policy name </th>
<th> Remarks </th>
</tr>
</thead>
<tbody>
<tr>
<td>AliyunECSFullAccess</td>
<td> Permissions to manage ECS </td>
</tr>
<tr>
<td>AliyunVPCFullAccess</td>
<td> Permissions for managing VPC networks </td>
</tr>
<tr>
<td>AliyunROSFullAccess</td>
<td> Manage permissions for Resource Orchestration Services (ROS) </td>
</tr>
<tr>
<td>AliyunComputeNestUserFullAccess</td>
<td> Manage user-side permissions for the compute nest service (ComputeNest) </td>
</tr>
</tbody>
</table>

<h2> Deployment Services </h2>

<ol>
<li> Click <a href = "https://computenest.console.aliyun.com/service/palworld/deploy?ServiceId=service-5ad5f65c6c5f4c3fb838"> Deployment Link </a> to go to the service instance deployment page. Enter the parameters as prompted.
<img src="deploy_1.jpg" alt="" /></li>
<li><p> The deployment parameters need to be API-KEY. <strong><a href = "https://bailian.console.aliyun.com/"> Log in to the console </a></strong>, hover the cursor over the pedestrian icon in the upper right corner, and click <strong>API-KEY</strong>.
<img src="bailian1.png" alt="" /></p>

<p> Click <strong> Create My API-KEY</strong> and copy it for standby. API-KEY is personal confidential information, do not disclose. If Bailian is not activated, please click <a href = "https://help.aliyun.com/zh/model-studio/getting-started/first-api-call-to-qwen?spm=a2c4g.11186623.help-menu-2400256.d_0_1_0.5a06b0a8lg5WY2#5058e161041ps"> Activate Bailian Model Service </a> to complete the activation.
<img src="bailian2.png" alt="" /></p></li>
<li><p> Click <strong> Create Now </strong> after confirming the order is complete. </p></li>
<li><p> After the deployment is completed, you can start using the service. Enter the service instance details and click Address to access.
<img src="result.png" alt="result.png" /></p></li>
<li><p> Register an account and log in to the service.
<img src="login.jpg" alt="login.png" /></p></li>
<li><p> Start your AI conversation.
<img src="use_0.png" alt="login.png" /></p></li>
</ol>

<p>DeepSeek-R1 open thinking mode <a href = "https://www.zhihu.com/question/10904918866/answer/99141193645"> refer to the community plan </a></p>
