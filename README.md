<h2>🧩🧩 Guide to solve basic kubernetes problems 🧩🧩</h1>
<h2>  🌼Kubernetes is a container orchestration tool ,and while working with it errors are part of it ,but it would be time saving if we knew where to debug & fix the issue, as for a beginner things might get overwhelming.
  
![Static Badge](https://img.shields.io/badge/pods-purple)
  
![Static Badge](https://img.shields.io/badge/kubernetes-cluster-red)


![Static Badge](https://img.shields.io/badge/kubernetes-debugging-green)


</h2> 
<h3> <STRONG> What is Kubernetes ?</STRONG></h3>
<h3> 🔌 Kuberenetes which is also widely refered to as  <kbd> k8s </kbd>  is open-source container orchestration  technology used for managing your applications & automating deployments of software . Initially it was founded & owned by <kbd> Google </kbd>kbd>, but now is maintained by  <kbd> Cloud Native Computing Foundation </kbd></h3>
<h3>You can read more about it it here   <a href="https://kubernetes.io/" target="_blank">Kubernetes Overview</a>   </h3>

<h3> <Strong> Why Kubernetes debugging is helpful ? </Strong> </h3>
<h3> When deploying application to kubernetes clusters , which is itself a complex system has multiple components involved , at times during  
  
  ![Static Badge](https://img.shields.io/badge/deploying-pink)  ,
![Static Badge](https://img.shields.io/badge/managing-magenta)  , 
  ![Static Badge](https://img.shields.io/badge/running-pink) 
  you may face common issues listed below , debugging provides essential information to track down the issue &  ![Static Badge](https://img.shields.io/badge/fix-grey)


 

 
<br> </br>

<h2><BOLD> Here are 5 common k8s failures and how to fix them 🛠️  </BOLD> </h2>
  
 ![Screenshot](s1.png)



<ol>  <h3>  🏷𝟏) 𝐈𝐦𝐚𝐠𝐞-𝐩𝐮𝐥𝐥 𝐛𝐚𝐜𝐤 𝐨𝐟𝐟 </ol> </h3>
<ol>  <h3>  🏷2) 𝐂𝐫𝐚𝐬𝐡-𝐥𝐨𝐨𝐩 𝐛𝐚𝐜𝐤 𝐨𝐟𝐟 </ol> </h3>
<ol>  <h3>  🏷3) 𝐅𝐚𝐢𝐥𝐮𝐫𝐞 𝐰𝐢𝐭𝐡 𝐄𝐱𝐢𝐭 𝐜𝐨𝐝𝐞 :𝟏  </ol> </h3>
<ol>  <h3>  🏷4) 𝐅𝐚𝐢𝐥𝐮𝐫𝐞 𝐰𝐢𝐭𝐡 𝐄𝐱𝐢𝐭 𝐜𝐨𝐝𝐞 :𝟏𝟐𝟓 </ol> </h3>
<ol>  <h3>  🏷5) 𝐏𝐨𝐝 /𝐍𝐨𝐝𝐞 𝐧𝐨𝐭 𝐫𝐞𝐚𝐝𝐲 </ol> </h3>

<h3>🌵 1) 𝐈𝐦𝐚𝐠𝐞-𝐩𝐮𝐥𝐥 𝐛𝐚𝐜𝐤 𝐨𝐟𝐟 </h3> 

![Static Badge](https://img.shields.io/badge/Issue%3A1-yellow)

<summary> ~ Check for 𝙄𝙢𝙖𝙜𝙚 𝙥𝙪𝙡𝙡 𝙥𝙤𝙡𝙞𝙘𝙮 , 𝙥𝙚𝙧𝙢𝙞𝙨𝙨𝙞𝙤𝙣 𝙩𝙤 𝙥𝙪𝙡𝙡 𝙛𝙧𝙤𝙢 𝙧𝙚𝙥𝙤𝙨𝙞𝙩𝙤𝙧𝙮,𝙘𝙤𝙧𝙧𝙚𝙘𝙩 𝙞𝙢𝙖𝙜𝙚 𝙣𝙖𝙢𝙚 𝙖𝙡𝙤𝙣𝙜 𝙬𝙞𝙩𝙝 𝙩𝙖𝙜. <summary>

<summary> <strong> Useful Commands 🔮 </strong> </summary> 
<ol> Kubectl describe po  <kbd> podname </kbd> </ol>
<ol> Kubectl get po <kbd> podname </kbd> </ol>
<ol> Kubectl apply -f deployment <kbd> File name </kbd> </ol>
<br> </br>

<h3>🌵2) 𝐂𝐫𝐚𝐬𝐡-𝐥𝐨𝐨𝐩 𝐛𝐚𝐜𝐤 𝐨𝐟𝐟 </h3>

![Static Badge](https://img.shields.io/badge/Issue%3A2-yellow)

<summary>~ Check for 𝘾𝙤𝙧𝙧𝙚𝙘𝙩 𝙞𝙢𝙖𝙜𝙚 𝙣𝙖𝙢𝙚 𝙖𝙡𝙤𝙣𝙜 𝙬𝙞𝙩𝙝 𝙩𝙖𝙜 , 𝙚𝙣𝙤𝙪𝙜𝙝 𝙧𝙚𝙨𝙤𝙪𝙧𝙘𝙚 𝙘𝙤𝙣𝙨𝙩𝙧𝙖𝙞𝙣𝙩𝙨,𝙢𝙞𝙨𝙘𝙤𝙣𝙛𝙞𝙜𝙪𝙧𝙖𝙩𝙞𝙤𝙣 𝙤𝙛 𝙚𝙣𝙫𝙞𝙧𝙤𝙣𝙢𝙚𝙣𝙩 𝙫𝙖𝙧𝙞𝙖𝙗𝙡𝙚𝙨 , 𝙖𝙥𝙥𝙡𝙞𝙘𝙖𝙩𝙞𝙤𝙣 𝙛𝙖𝙞𝙡𝙪𝙧𝙚 𝙗𝙚𝙘𝙖𝙪𝙨𝙚 𝙤𝙛 ( 𝙛𝙖𝙞𝙡 𝙩𝙤 𝙗𝙪𝙞𝙡𝙙 𝙟𝙖𝙧 𝙛𝙞𝙡𝙚𝙨 , 𝙞𝙨𝙨𝙪𝙚𝙨 𝙬𝙝𝙞𝙡𝙚 𝙗𝙪𝙞𝙡𝙙𝙞𝙣𝙜 𝙙𝙤𝙘𝙠𝙚𝙧 𝙞𝙢𝙖𝙜𝙚. <summary>

<summary> <strong> Useful Commands 🔮 </strong> </summary> 
<ol> Kubectl describe po  <kbd> podname </kbd> </ol>
<ol> Kubectl logs  <kbd> logs  podname </kbd> </ol>
<ol> Also to check if enough resources are allocated (memory) </ol>
<br> </br>

<h3>🌵 3) 𝐅𝐚𝐢𝐥𝐮𝐫𝐞 𝐰𝐢𝐭𝐡 𝐄𝐱𝐢𝐭 𝐜𝐨𝐝𝐞 :𝟏  </h3>

![Static Badge](https://img.shields.io/badge/Issue%3A3-yellow)

<summary>~ Check for 𝘼𝙥𝙥𝙡𝙞𝙘𝙖𝙩𝙞𝙤𝙣 𝙘𝙤𝙙𝙚 𝙘𝙧𝙖𝙨𝙝𝙚𝙨 , 𝙞𝙣𝙘𝙤𝙧𝙧𝙚𝙘𝙩 𝙚𝙣𝙫𝙞𝙧𝙤𝙣𝙢𝙚𝙣𝙩 𝙫𝙖𝙧𝙞𝙖𝙗𝙡𝙚𝙨, 𝙞𝙣𝙨𝙪𝙛𝙛𝙞𝙘𝙞𝙚𝙣𝙩 𝙛𝙞𝙡𝙚 𝙥𝙚𝙧𝙢𝙞𝙨𝙨𝙞𝙤𝙣𝙨. </summary>

<summary> <strong> Useful Commands 🔮 </strong> </summary> 
<ol> Kubectl logs <kbd> podname </kbd> </ol>
<ol> Kubectl get po <kbd> podname </kbd> </ol>
<ol> Kubectl apply -f deployment <kbd> podname </kbd> </ol>
<ol> Lookout for any exceptions in logs /missing variables at code level as well . </ol>
<br> </br>

<h3>🌵 4) 𝐅𝐚𝐢𝐥𝐮𝐫𝐞 𝐰𝐢𝐭𝐡 𝐄𝐱𝐢𝐭 𝐜𝐨𝐝𝐞 :𝟏𝟐𝟓</h3>

![Static Badge](https://img.shields.io/badge/Issue%3A4-yellow)

<summary> ~ Check for 𝙞𝙣𝙘𝙤𝙧𝙧𝙚𝙘𝙩 𝙛𝙞𝙡𝙚 𝙥𝙚𝙧𝙢𝙞𝙨𝙨𝙞𝙤𝙣𝙨 , 𝙚𝙭𝙘𝙚𝙥𝙩𝙞𝙤𝙣𝙨 𝙙𝙪𝙧𝙞𝙣𝙜 𝙗𝙤𝙤𝙩𝙞𝙣𝙜 𝙪𝙥 𝙤𝙛 𝙥𝙤𝙙 </summary>

<summary> <strong> Useful Commands 🔮 </strong> </summary> 

<ol> Kubectl logs <kbd> podname </kbd> </ol>
<ol> Kubectl describe <kbd> podname </kbd> </ol>
<br> </br>

<h3>🌵5) 𝐏𝐨𝐝/𝐍𝐨𝐝𝐞 𝐧𝐨𝐭 𝐫𝐞𝐚𝐝𝐲 </h3>

![Static Badge](https://img.shields.io/badge/Issue%3A5-yellow)

<summary>~ Check for 𝙉𝙚𝙩𝙬𝙤𝙧𝙠 𝘾𝙤𝙣𝙣𝙚𝙘𝙩𝙞𝙫𝙞𝙩𝙮 , 𝙚𝙣𝙤𝙪𝙜𝙝 𝙧𝙚𝙨𝙤𝙪𝙧𝙘𝙚 𝙖𝙡𝙡𝙤𝙘𝙖𝙩𝙞𝙤𝙣 ,𝙪𝙣𝙝𝙚𝙖𝙡𝙩𝙝𝙮 𝙥𝙧𝙤𝙘𝙚𝙨𝙨𝙚𝙨  </summary>

<summary> <strong> Useful Commands 🔮 </strong> </summary>  
<ol> Kubectl logs <kbd> podname </kbd> </ol>
<ol> Kubectl get po <kbd> podname </kbd> and check for its <kbd> state </kbd> </ol>
<ol> Increase system resource usage </ol>

________________________________________________________________________________________________________________________________________________________________________________________________________________
