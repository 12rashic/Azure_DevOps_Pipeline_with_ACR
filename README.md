<h1>🧩🧩 Must Know debuggings working with kubernetes cluster 🧩🧩</h1>
<h2>  🌼Kubernetes is a container orchestration tool ,and while working with it errors are part of it , but it would be time saving if we knew where to debug & fix the issue, as for a beginner things might get overwhelming. </h2> 
<h3> <STRONG> What is Kubernetes ?</STRONG></h3>
<h3> 🔌 Kuberenetes which is also widely refered to as  <kbd> k8s </kbd>  is open-source container orchestration  technology used for managing your applications & automating deployments of software . Initially it wa founded & owned by <kbd> Google </kbd>kbd>, but now is maintained by  <kbd> Cloud Native Computing Foundation </kbd></h3>
<H3><summary></H3>Here are 5 common k8s failures and how to fix them 🛠️ </summary> <h3> </summary>

<ol>   🏷𝟭) 𝗜𝗺𝗮𝗴𝗲-𝗽𝘂𝗹𝗹 𝗯𝗮𝗰𝗸 𝗼𝗳𝗳   </ol>
<ol>   🏷2) 𝘾𝙧𝙖𝙨𝙝-𝙇𝙤𝙤𝙥 𝙗𝙖𝙘𝙠 𝙤𝙛𝙛   </ol>
<ol>   🏷3) 𝙁𝙖𝙞𝙡𝙪𝙧𝙚 𝙬𝙞𝙩𝙝 𝙀𝙭𝙞𝙩 𝙘𝙤𝙙𝙚 1   </ol> 
<ol>   🏷4) 𝙁𝙖𝙞𝙡𝙪𝙧𝙚 𝙬𝙞𝙩𝙝 𝙀𝙭𝙞𝙩 𝙘𝙤𝙙𝙚125 </ol>
<ol>   🏷5) 𝙋𝙤𝙙/𝙉𝙤𝙙𝙚 𝙉𝙤𝙩 𝙍𝙚𝙖𝙙𝙮 </ol>

<h3>🌵𝟭) 𝗜𝗺𝗮𝗴𝗲-𝗽𝘂𝗹𝗹 𝗯𝗮𝗰𝗸 𝗼𝗳𝗳 </h3> 
<summary> ~ Check for 𝙄𝙢𝙖𝙜𝙚 𝙥𝙪𝙡𝙡 𝙥𝙤𝙡𝙞𝙘𝙮 , 𝙥𝙚𝙧𝙢𝙞𝙨𝙨𝙞𝙤𝙣 𝙩𝙤 𝙥𝙪𝙡𝙡 𝙛𝙧𝙤𝙢 𝙧𝙚𝙥𝙤𝙨𝙞𝙩𝙤𝙧𝙮,𝙘𝙤𝙧𝙧𝙚𝙘𝙩 𝙞𝙢𝙖𝙜𝙚 𝙣𝙖𝙢𝙚 𝙖𝙡𝙤𝙣𝙜 𝙬𝙞𝙩𝙝 𝙩𝙖𝙜. <summary>

<summary> 𝙐𝙨𝙚𝙛𝙪𝙡 𝙘𝙤𝙢𝙢𝙖𝙣𝙙𝙨 🔮 </summary>summary>
Kubectl describe po  <kbd> podname </kbd>
Kubectl get po <kbd> podname </kbd>
Kubectl apply -f <deployment <kbd> File name </kbd>

<h3>🌵2) 𝘾𝙧𝙖𝙨𝙝-𝙇𝙤𝙤𝙥 𝙗𝙖𝙘𝙠 𝙤𝙛𝙛 </h3>
<summary>~ Check for 𝘾𝙤𝙧𝙧𝙚𝙘𝙩 𝙞𝙢𝙖𝙜𝙚 𝙣𝙖𝙢𝙚 𝙖𝙡𝙤𝙣𝙜 𝙬𝙞𝙩𝙝 𝙩𝙖𝙜 , 𝙚𝙣𝙤𝙪𝙜𝙝 𝙧𝙚𝙨𝙤𝙪𝙧𝙘𝙚 𝙘𝙤𝙣𝙨𝙩𝙧𝙖𝙞𝙣𝙩𝙨,𝙢𝙞𝙨𝙘𝙤𝙣𝙛𝙞𝙜𝙪𝙧𝙖𝙩𝙞𝙤𝙣 𝙤𝙛 𝙚𝙣𝙫𝙞𝙧𝙤𝙣𝙢𝙚𝙣𝙩 𝙫𝙖𝙧𝙞𝙖𝙗𝙡𝙚𝙨 , 𝙖𝙥𝙥𝙡𝙞𝙘𝙖𝙩𝙞𝙤𝙣 𝙛𝙖𝙞𝙡𝙪𝙧𝙚 𝙗𝙚𝙘𝙖𝙪𝙨𝙚 𝙤𝙛 ( 𝙛𝙖𝙞𝙡 𝙩𝙤 𝙗𝙪𝙞𝙡𝙙 𝙟𝙖𝙧 𝙛𝙞𝙡𝙚𝙨 , 𝙞𝙨𝙨𝙪𝙚𝙨 𝙬𝙝𝙞𝙡𝙚 𝙗𝙪𝙞𝙡𝙙𝙞𝙣𝙜 𝙙𝙤𝙘𝙠𝙚𝙧 𝙞𝙢𝙖𝙜𝙚. <summary>

<summary> 𝙐𝙨𝙚𝙛𝙪𝙡 𝙘𝙤𝙢𝙢𝙖𝙣𝙙𝙨 🔮 </summary>
Kubectl describe po  <kbd> podname </kbd>
Kubectl logs  <kbd> logs  podname </kbd>
Also to check if enough resources are allocated (memory)

________________________________________________________________________________________________________________________________________________________________________________________________________________
